### **Resumen de Capabilities en Linux** 🐧

Las **capabilities** en Linux son una forma de **dividir los privilegios de root** en permisos más pequeños y específicos, mejorando la **seguridad** del sistema. Permiten que un proceso tenga ciertos privilegios sin necesidad de ejecutarse como `root`. Esto reduce el impacto de errores y vulnerabilidades.

- **¿Qué resuelven?**  
    Aplican el **principio de mínimos privilegios**, evitando que un proceso tenga más permisos de los necesarios.

#### **Ejemplos Comunes:**

- **`CAP_NET_BIND_SERVICE`**: Permite abrir puertos menores a 1024 sin ser root.
- **`CAP_SYS_TIME`**: Permite ajustar la hora del sistema.
- **`CAP_SETUID`**: Permite cambiar el UID del proceso.
- **`CAP_NET_RAW`**: Habilita el uso de paquetes en bruto (por ejemplo, ICMP para ping).

#### **Comandos útiles:**

- **Ver capabilities de un binario:**
`getcap /usr/bin/ping
`
Asignar capabilities a un archivo:
`sudo setcap cap_net_bind_service=+ep /usr/bin/myapp
`
Eliminar capabilities:
`sudo setcap -r /usr/bin/myapp
`
#### **Impacto en Ciberseguridad:**

- **Escalación de privilegios:** Si un binario con `setuid` tiene malas configuraciones o capacidades elevadas, un atacante puede explotarlo.
- **Mitigación:** Permite limitar los privilegios de procesos críticos, reduciendo el impacto de compromisos.
