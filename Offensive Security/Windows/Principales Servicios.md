### 1. **RDP (Remote Desktop Protocol)**

- **Servicio**: Permite conexiones remotas a través de la interfaz gráfica de un sistema Windows.
- **Puerto**: **3389**
- **Uso**: Conectar de forma remota a escritorios y controlar sistemas Windows de manera gráfica.

### 2. **SMB (Server Message Block)**

- **Servicio**: Facilita el intercambio de archivos, impresoras y recursos entre dispositivos en una red.
- **Puerto**: **445** (SMBv2 y SMBv3), anteriormente también utilizaba los puertos **137-139** (NetBIOS).
- **Uso**: Compartición de archivos y periféricos (impresoras, carpetas) en redes Windows.

### 3. **WinRM (Windows Remote Management)**

- **Servicio**: Administración remota de sistemas Windows, permite ejecutar comandos de manera remota.
- **Puerto**: **5985** (HTTP) y **5986** (HTTPS).
- **Uso**: Gestión remota de servidores Windows, similar a SSH en Linux pero con un enfoque en administración por comandos.

### 4. **WebDAV (Web Distributed Authoring and Versioning)**

- **Servicio**: Permite la edición y administración de archivos en un servidor web (como un servidor IIS).
- **Puerto**: **80** (HTTP) y **443** (HTTPS).
- **Uso**: Facilita el acceso remoto a archivos y su administración a través de un navegador o cliente WebDAV.

### 5. **IIS (Internet Information Services)**

- **Servicio**: Es el servidor web nativo de Windows para alojar sitios web y aplicaciones web.
- **Puerto**: **80** (HTTP) y **443** (HTTPS).
- **Uso**: Alojamiento de sitios web, servicios web y aplicaciones en entornos Windows.

### 6. **WMI (Windows Management Instrumentation)**

- **Servicio**: Permite la administración y monitorización de dispositivos y aplicaciones en una red de Windows.
- **Puerto**: **135** (RPC) más un puerto dinámico que se asigna al momento.
- **Uso**: Herramienta poderosa para la administración y recopilación de información de sistemas Windows.

### 7. **DNS (Domain Name System)**

- **Servicio**: Traduce nombres de dominio en direcciones IP.
- **Puerto**: **53** (UDP/TCP).
- **Uso**: Resolución de nombres en redes Windows (así como en otras redes).

### 8. **DHCP (Dynamic Host Configuration Protocol)**

- **Servicio**: Asigna dinámicamente direcciones IP a dispositivos en la red.
- **Puerto**: **67** (servidor) y **68** (cliente) (UDP).
- **Uso**: Configuración automática de direcciones IP y otros parámetros de red a dispositivos en redes Windows.

### 9. **LDAP (Lightweight Directory Access Protocol)**

- **Servicio**: Protocolo utilizado para acceder y administrar servicios de directorio, como Active Directory.
- **Puerto**: **389** (LDAP) y **636** (LDAPS - LDAP sobre SSL).
- **Uso**: Autenticación y administración de usuarios en Active Directory.

### 10. **Kerberos**

- **Servicio**: Protocolo de autenticación utilizado en redes Windows para verificar la identidad de usuarios.
- **Puerto**: **88** (TCP/UDP).
- **Uso**: Autenticación segura de usuarios en entornos de dominio Windows.