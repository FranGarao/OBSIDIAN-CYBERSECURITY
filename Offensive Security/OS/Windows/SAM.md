### **SAM (Security Account Manager)**

- **Descripción**: El **Security Account Manager (SAM)** es una base de datos en sistemas Windows que almacena las credenciales de usuarios locales, como **hashes de contraseñas** y datos de las cuentas de usuario. El SAM es esencial para la gestión de cuentas y autenticación local en sistemas Windows.
    
- **Ubicación**:
    
    - Se encuentra en **%SystemRoot%/system32/config/SAM**.
    - No es accesible mientras el sistema operativo está en funcionamiento debido a que está bloqueado por el sistema.
- **Seguridad**:
    
    - **Cifrado**: Los datos del SAM están cifrados mediante una clave del sistema que se almacena en el registro de Windows, específicamente en la ruta **SYSTEM**.
    - **Hashes**: Las contraseñas no se almacenan en texto plano, sino en forma de **hashes NTLM** o **LM** (en versiones antiguas), lo que hace que sean más difíciles de recuperar directamente, pero susceptibles a ataques de fuerza bruta o diccionario si se obtienen los hashes.
- **Acceso**:
    
    - **Dumping del SAM**: Las herramientas de hacking pueden extraer hashes de contraseñas del SAM utilizando exploits como **mimikatz**, **PwDump**, o **Metasploit**.
    - **SAM en modo seguro o con un live CD**: El SAM puede ser accedido si el sistema está arrancado desde un entorno alternativo (como un **Live CD**) o con privilegios de administrador.
- **Herramientas**:
    
    - **mimikatz**: Puede extraer hashes y otras credenciales directamente de la memoria del sistema, incluyendo los del SAM.
    - **Cain & Abel**: Utilizada para extraer hashes del SAM y realizar ataques de fuerza bruta o diccionario.
    - **John the Ripper**: Herramienta común para crackear los hashes NTLM extraídos.
- **Comandos**:
```shell
# Para acceder a los hashes en un sistema comprometido
secretsdump.py <usuario>@<ip>  # (Usa impacket)

```

# Notas

- **Dumping de SAM** es una técnica común usada por atacantes tras una escalada de privilegios para obtener credenciales de otros usuarios.
- **Protección del SAM**: Habilitar **BitLocker**, **Windows Defender Credential Guard** o usar contraseñas fuertes dificulta la extracción de hashes y su posterior cracking.

# Vulns

- **LSASS (Local Security Authority Subsystem Service)**: Herramientas como **mimikatz** pueden acceder a la memoria de LSASS para extraer hashes de contraseñas almacenados temporalmente.

**nmap scripts**

- **nmap --script smb-os-discovery**: Puede identificar versiones vulnerables de SMB que permiten el dumping del SAM.

**metasploit**

- **post/windows/gather/smart_hashdump**: Permite extraer los hashes de SAM a través de Metasploit.
