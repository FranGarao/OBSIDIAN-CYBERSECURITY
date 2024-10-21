### **Telnet**

- **Descripción**: Protocolo de red que permite la administración remota de dispositivos, pero **sin cifrado**, lo que lo hace inseguro para entornos modernos.
    
- **Puertos**:
    - **23** por defecto.
    
- **Seguridad**: Telnet no cifra los datos, incluidas las credenciales, por lo que es vulnerable a la interceptación. Se recomienda usar **SSH** en lugar de Telnet.

- **Servicios**:
    - **inetd (en sistemas Unix)**
    - **xinetd**

- **Comandos**:
```
telnet hostname
telnet hostname 23
```