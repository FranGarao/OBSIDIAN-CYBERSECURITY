### **SMB (Server Message Block)**

- **Descripción**: Protocolo utilizado principalmente en redes Windows para compartir archivos, impresoras y otros recursos entre dispositivos en la misma red. Es un protocolo de capa de aplicación que facilita la transferencia de datos y la interacción entre dispositivos.
    
- **Puertos**:
    - **445** por defecto (SMB directo).
    - **137-139** para NetBIOS sobre TCP/IP (antiguamente utilizado en versiones más antiguas de SMB).

- **Seguridad**: SMB por defecto no cifra los datos, pero las versiones más recientes (como **SMBv3**) soportan cifrado y autenticación más seguras. Para mejorar la seguridad:
    - **SMBv3**: Introduce cifrado AES y otras mejoras de seguridad.
    - **Kerberos**: Autenticación segura en entornos de dominio Active Directory.
    - **NTLM**: Autenticación basada en desafío/respuesta.

- **Servicios**:
    - **Samba** (en sistemas Linux/Unix para compatibilidad con SMB en redes Windows).
    - **SMB (nativo en Windows)**.
    - **CIFS (Common Internet File System)**: Una versión más antigua de SMB, aunque todavía utilizada en algunos entornos.

- **Comandos**:
```
smbclient //server/share
net view \\server
net use X: \\server\share
```