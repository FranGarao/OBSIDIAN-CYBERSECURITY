### **IMAP (Internet Message Access Protocol)**

- **Descripción**: Protocolo utilizado para acceder a correos electrónicos almacenados en un servidor desde clientes locales.
    
- **Puertos**:
    - **143** por defecto.
    - **993** para IMAPS (IMAP sobre SSL/TLS).
    
- **Seguridad**: IMAP no cifra los datos por defecto. Para asegurar la transmisión:
    - **IMAPS**: Usa SSL/TLS para cifrar el acceso al correo.

- **Servicios**:
    - **Dovecot**
    - **Cyrus IMAP**
    - **Zimbra**
    
- **Comandos**:
```
telnet imap.example.com 143
openssl s_client -connect imap.example.com:993
```