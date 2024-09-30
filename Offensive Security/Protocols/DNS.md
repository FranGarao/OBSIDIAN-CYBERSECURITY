### **DNS (Domain Name System)**

- **Descripción**: Protocolo que traduce nombres de dominio en direcciones IP, esencial para la navegación en internet.
    
- **Puertos**:
    - **53** por defecto (UDP/TCP).
    
- **Seguridad**: DNS por sí mismo no es seguro y es susceptible a ataques como envenenamiento de caché. Para asegurar la comunicación:
    - **DNSSEC**: Añade autenticación de origen de los datos mediante firmas digitales.

- **Servicios**:
    - **BIND (Berkeley Internet Name Domain)**
    - **Unbound**
    - **PowerDNS**
    
- **Comandos**:
```
nslookup example.com
dig example.com
host example.com
```