El _tunneling_ es una técnica utilizada en redes de computadoras que permite el envío de datos entre dos redes utilizando una red intermedia, encapsulando el tráfico en un protocolo diferente al que normalmente usaría. Esta técnica es esencial para asegurar o permitir la transmisión de paquetes de datos que normalmente no serían compatibles o admitidos en esa red intermedia.

### Tipos de tunneling:

1. **Tunneling voluntario**: Es iniciado y finalizado por el usuario o cliente. Los dispositivos finales crean los túneles de forma manual o mediante software.
    
2. **Tunneling compulsorio**: La creación del túnel es gestionada por el servidor o el proveedor de servicios. El usuario final no participa en la configuración del túnel.
    
3. **Tunneling punto a punto (PPTP)**: Este es un protocolo más antiguo utilizado para crear VPN. Encapsula los datos en un formato IP que se puede enviar sobre una red pública como Internet.
    
4. **Tunneling capa 2 (L2TP)**: Trabaja a nivel de enlace de datos (Capa 2 del modelo OSI) y es comúnmente combinado con IPsec para proporcionar seguridad adicional, permitiendo la transmisión segura de datos a través de redes públicas.
    
5. **Tunneling capa 3 (IPsec)**: Operando a nivel de red, IPsec es un protocolo que cifra y asegura la comunicación a nivel de capa de red. Se usa ampliamente para crear túneles seguros en redes IP.
    
6. **Tunneling SSH (Secure Shell)**: Se utiliza para encapsular y redirigir tráfico a través de un canal SSH seguro, garantizando que los datos se transmitan de manera cifrada.
    
7. **Tunneling GRE (Generic Routing Encapsulation)**: GRE encapsula una variedad de protocolos de capa 3 dentro de túneles IP, permitiendo la transmisión de datos a través de redes IP de manera sencilla, pero sin cifrado.
    

### Aplicaciones del tunneling:

- **VPNs (Virtual Private Networks)**: El uso más común del tunneling, permitiendo que los usuarios creen redes privadas seguras a través de Internet.
- **Tráfico IPv6 sobre IPv4**: El tunneling se utiliza para transmitir paquetes IPv6 sobre redes que solo soportan IPv4.
- **Reducción de restricciones geográficas**: Usuarios pueden acceder a contenido bloqueado geográficamente usando VPNs.
- **Seguridad y privacidad**: A través de la encapsulación y el cifrado, el tunneling protege la privacidad y seguridad de los datos en tránsito.