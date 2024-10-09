### **ADS (Alternate Data Streams)**

- **Descripción**: Los **Alternate Data Streams** son una característica del sistema de archivos **NTFS** que permite almacenar información adicional (como metadatos o datos ocultos) dentro de un archivo sin alterar su tamaño visible ni su contenido principal. Esto facilita el almacenamiento de datos secundarios junto con un archivo principal sin que sea evidente para el usuario.
    
- **Sistema de archivos**:
    
    - **NTFS** (New Technology File System): El sistema de archivos donde se encuentra disponible la funcionalidad ADS.
- **Seguridad**: Aunque ADS puede ser útil para almacenar metadatos, también puede ser utilizado con fines maliciosos, como **ocultar malware** o código malicioso en archivos inofensivos. Debido a que los ADS no son visibles de forma normal, pueden evadir la detección en algunos sistemas de análisis.
    
    - **Problemas de seguridad**: ADS puede ocultar ejecutables maliciosos sin modificar el tamaño del archivo original.
    - **Herramientas de detección**: Para identificar y gestionar ADS, es necesario usar herramientas específicas como `streams.exe` o `dir /r` en la línea de comandos de Windows.
- **Uso común**:
    
    - **Metadatos ocultos**: Se pueden utilizar para almacenar información adicional relacionada con archivos, como detalles de autoría o historial de modificaciones.
    - **Exploits potenciales**: Utilizado a veces por atacantes para ocultar scripts o malware que se ejecutan desde un archivo aparentemente benigno.
- **Comandos**:
	```powershell
	notepad nothing.txt:secret.txt
	```
To hide a payload:
```powershell
#Create
payload.exe > nothing.txt:executable_name.exe

#Create a simbolic link
mklink wupdate.exe C:\Temp\nothing.txt:executable_name.exe

#Execute
wupdate

#Isnt works
start nothing.txt:executable_name.exe
```


# Notas

- **ADS** son invisibles a través de exploradores de archivos convencionales, por lo que requieren comandos específicos para ser detectados.
- **Streams.exe** es una herramienta de Sysinternals que facilita la identificación y eliminación de ADS en archivos.

# Vulns

- **Uso malicioso**: Los ADS pueden ser utilizados por atacantes para ocultar archivos maliciosos sin alterar la visibilidad o el tamaño de los archivos en el sistema.

**nmap scripts**

- ADS no tiene scripts de Nmap directamente, pero la **detección de malware** oculto en ADS puede ser parte de un análisis de seguridad más amplio.

**metasploit**

- **ADS abuse**: Los atacantes pueden abusar de ADS para esconder cargas maliciosas, pero Metasploit en sí no tiene módulos específicos para ADS.