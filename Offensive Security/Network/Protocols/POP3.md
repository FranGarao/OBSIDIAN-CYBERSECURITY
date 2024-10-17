### **POP3 (Post Office Protocol version 3)**

- **Descripción**: Protocolo utilizado para la descarga de correos electrónicos desde un servidor al cliente de correo.
    
- **Puertos**:
    - **110** por defecto.
    - **995** para POP3S (POP3 sobre SSL/TLS).
    
- **Seguridad**: POP3 no cifra los datos por defecto. Para mejorar la seguridad:
    - **POP3S**: Utiliza SSL/TLS para cifrar el acceso al correo.

- **Servicios**:
    - **Dovecot**
    - **Courier**
    - **Zimbra**

    
- **Comandos**:
```
telnet pop.example.com 110
openssl s_client -connect pop.example.com:995
```