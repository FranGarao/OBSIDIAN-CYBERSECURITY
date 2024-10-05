### **WinRM (Windows Remote Management)**

- **Descripción**: Protocolo de red diseñado para permitir la gestión remota de sistemas Windows. Utiliza la implementación de WS-Management de Microsoft, que es un estándar basado en SOAP (Simple Object Access Protocol), para intercambiar información de gestión entre sistemas. WinRM es especialmente útil para la administración de servidores remotos sin necesidad de acceder físicamente al sistema.
    
- **Puertos**:
    - **5985**: Puerto por defecto para conexiones HTTP.
    - **5986**: Puerto por defecto para conexiones HTTPS (más seguro).

- **Seguridad**:
    - **Kerberos**: Protocolo predeterminado para la autenticación en entornos de dominio.
    - **CredSSP**: Proporciona autenticación delegada segura, ideal para conexiones remotas.
    - **Cifrado TLS**: WinRM admite la protección de las comunicaciones mediante TLS, especialmente cuando se utiliza el puerto 5986 para conexiones HTTPS.
    - **Control de acceso basado en roles (RBAC)**: Se puede configurar para limitar el acceso de acuerdo con las funciones de los usuarios.
    - **VPN**: Recomendado para encapsular y asegurar el tráfico WinRM, reduciendo la exposición a redes públicas.

- **Servicios**:
    - **Windows Remote Management (WinRM)**: Servicio en sistemas Windows que gestiona las conexiones remotas y las solicitudes de administración.

- **Tools**:
    - **PowerShell**: Herramienta principal para interactuar con WinRM. Ejemplo de uso:
```
Enter-PSSession -ComputerName nombre_servidor -Credential usuario

winrs -r:hostname comando

Invoke-Command -ComputerName nombre_servidor -ScriptBlock {comando}

crackmapexec (brute-force)

evil-winrm (to obtain a command shell session on the target system)
```

**Vulnerabilidades**:
- **CVE-2021-31166**: Vulnerabilidad en el protocolo HTTP de WinRM que permite la ejecución remota de código (RCE). Afecta a Windows 10 y Windows Server.
- **CVE-2020-0601**: Vulnerabilidad en cómo WinRM valida certificados, permitiendo a los atacantes realizar ataques man-in-the-middle (MITM).