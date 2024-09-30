### **RDP (Remote Desktop Protocol)**

- **Descripción**: Protocolo de red que permite a los usuarios conectarse de forma remota a una computadora con Windows, proporcionándoles acceso a su escritorio y aplicaciones como si estuvieran físicamente frente a la máquina.
    
- **Puertos**:
    - **3389**: Puerto por defecto para conexiones RDP.

- **Seguridad**:
    - **CredSSP**: Cifrado de las credenciales durante el inicio de sesión.
    - **RDP sobre TLS**: Implementación que permite asegurar las conexiones RDP mediante cifrado TLS.
    - **VPN**: Se recomienda utilizar una VPN para encapsular y asegurar las conexiones RDP.

- **Servicios**:
    - **Remote Desktop Services (RDS)** en Windows.

- **Comandos**:
```
mstsc /v:hostname
rdesktop hostname
```