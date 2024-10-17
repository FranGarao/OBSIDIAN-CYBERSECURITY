### **RPC (Remote Procedure Call)**

- **Descripción**: Es un protocolo que permite a un programa solicitar un servicio desde otro programa ubicado en otra computadora en la red sin tener que entender los detalles de la red. Es ampliamente utilizado en sistemas distribuidos y en entornos Windows para permitir la comunicación entre aplicaciones y servicios.
    
- **Puertos**:
    - **135**: Puerto estándar para **Microsoft RPC Endpoint Mapper**, utilizado para asignar otros puertos dinámicos.
    - **Puertos dinámicos**: Una vez que se establece la conexión en el puerto 135, RPC asigna un puerto dinámico para la comunicación entre el cliente y el servidor. Estos puertos suelen estar en el rango **1024-65535**, aunque puede configurarse para usar un rango más restringido.


- **Seguridad**: RPC por sí solo no cifra las comunicaciones. Para mejorar la seguridad en entornos Windows, se suele utilizar junto con:
    - **Kerberos**: Para autenticación segura en dominios Active Directory.
    - **SSL/TLS**: Para cifrar la comunicación.


- **Servicios**:
    - **Microsoft RPC**: Utilizado en sistemas Windows para diversos servicios, incluyendo DCOM (Distributed Component Object Model).
    - **ONC RPC (Open Network Computing RPC)**: Implementación utilizada principalmente en sistemas Unix/Linux.

- **Comandos**:
```
rpcinfo
rpcping
```