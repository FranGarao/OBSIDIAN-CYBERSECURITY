### **SMTP (Simple Mail Transfer Protocol)**

- **Descripción**: Protocolo utilizado para el envío de correos electrónicos entre servidores y desde clientes de correo hacia el servidor.
    
- **Puertos**:
    - **25** por defecto.
    - **465** para SMTPS (SMTP con SSL/TLS).
    - **587** para envío autenticado con STARTTLS.
    
- **Seguridad**: SMTP no cifra los datos por defecto. Para mejorar la seguridad:
    - **SMTPS**: Utiliza SSL/TLS para cifrar la comunicación.
    - **STARTTLS**: Usa cifrado en el puerto 587 para asegurar la transmisión.

- **Servicios**:
    - **Postfix**
    - **Exim**
    - **Sendmail**
    - **Microsoft Exchange**

- **Comandos**:
```
telnet smtp.example.com 25
sendmail
```