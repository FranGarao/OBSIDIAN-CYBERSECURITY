### **(File Transfer Protocol)**

- **==Descripción**==: Protocolo de red utilizado para la transferencia de archivos entre un cliente y un servidor. Soporta modos de conexión activo y pasivo.
    
- **==Puertos==**:
    - **21** por defecto (control).
    - **20** para la transferencia de datos en modo activo.
    - **22** si usa SSH (SFTP).
- ==**Seguridad==**: FTP no cifra las credenciales ni los datos. Para mejorar la seguridad:
    - **SFTP (SSH File Transfer Protocol)**: Utiliza el puerto 22 y cifra tanto los datos como las credenciales mediante SSH.
    - **FTPS (FTP Secure)**: Utiliza SSL/TLS para cifrar la conexión (puerto 21 para control, puertos 989/990 para datos).
    
- **Servicios**:
	- **vsftpd**
	- **ProFTPD**
	- **FileZilla Server**

- **==Comandos**==:
```
ftp
ftp -?
dir
get
put
ls
mget
```


#Vulns 
anonymous access
```bash
ls -al /usr/share/nmap/scripts/ | grep ftp-*
#brute force
hydra -L /usr/share/metasploit-framework/data/wordlists/common_users.txt -P /usr/share/metasploit-framework/data/wordlists/unix_passwords.txt 10.10.10.10 -t 4 ftp
``` 

