### **LDAP (Lightweight Directory Access Protocol)**

- **Descripción**: Protocolo utilizado para acceder y administrar servicios de directorio, como **Active Directory**, que contienen información sobre usuarios, dispositivos y otros recursos de la red.
    
- **Puertos**:
    - **389**: Puerto por defecto para LDAP sin cifrar.
    - **636**: Puerto para LDAP sobre SSL/TLS (LDAPS).

- **Seguridad**: LDAP por defecto no es seguro. Para mejorar la seguridad:
    - **LDAPS**: Utiliza SSL/TLS para cifrar la comunicación.
    - **Kerberos**: Autenticación de usuarios en entornos de dominio.

- **Servicios**:
    - **Active Directory (AD)** en Windows.
    - **OpenLDAP** en sistemas Linux/Unix.

- **Comandos**:
```
ldapsearch -x -H ldap://hostname
ldapmodify -H ldaps://hostname
```