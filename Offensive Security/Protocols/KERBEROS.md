### **Kerberos**

- **Descripción**: Protocolo de autenticación seguro que utiliza la criptografía de clave simétrica para verificar la identidad de los usuarios en una red, y se usa principalmente en redes basadas en Windows para la autenticación en dominios.
    
- **Puertos**:
    - **88**: Puerto por defecto utilizado para la comunicación Kerberos.
    
- **Seguridad**: Kerberos es intrínsecamente seguro, ya que utiliza un sistema de **tickets** para autenticar a los usuarios sin transmitir contraseñas a través de la red.
    
- **Servicios**:
    - **KDC (Key Distribution Center)** en Active Directory (Windows).
    - **MIT Kerberos** en entornos Unix/Linux.

- **Comandos**:
```
kinit username
klist
```