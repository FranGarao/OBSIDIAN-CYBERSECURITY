(Secure Shell)

- **Descripción**: Protocolo para acceder de manera segura a dispositivos remotos mediante una conexión cifrada, utilizado para la administración remota de servidores.
    
- **Puertos**:
    - **22** por defecto.
    
- **Seguridad**: SSH cifra todo el tráfico, incluidas las credenciales, lo que lo hace muy seguro para la administración remota.

- **Servicios**:
    - **OpenSSH**
    - **Dropbear**
    - **PuTTY** (cliente)
    
- **Comandos**:
```
ssh user@hostname
ssh -p 22 user@hostname
```