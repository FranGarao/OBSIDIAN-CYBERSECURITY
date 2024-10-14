### **Resumen de Capabilities en Windows** 🪟

En **Windows**, las capacidades equivalentes se manejan a través de **privilegios y derechos de usuario**. Estos determinan lo que un proceso o usuario puede hacer en el sistema. Windows no usa el concepto de `setuid`, pero proporciona **privilegios específicos** a través de políticas.

#### **Ejemplos de Privilegios en Windows:**

- **SeBackupPrivilege**: Permite leer archivos sin restricciones de permisos (útil para copias de seguridad).
- **SeDebugPrivilege**: Permite depurar cualquier proceso en el sistema, incluso los que pertenecen a otros usuarios.
- **SeTcbPrivilege**: Concede al proceso permisos para actuar como parte del sistema operativo (muy peligroso).
- **SeShutdownPrivilege**: Permite apagar el sistema.

#### **Comandos útiles:**

- **Ver los privilegios de un usuario:**


**Agregar un privilegio a un usuario:** (requiere ser administrador)

Resumen de Capabilities en Linux 🐧

Las capabilities en Linux son una forma de dividir los privilegios de root en permisos más pequeños y específicos, mejorando la seguridad del sistema. Permiten que un proceso tenga ciertos privilegios sin necesidad de ejecutarse como root. Esto reduce el impacto de errores y vulnerabilidades.

    ¿Qué resuelven?
    Aplican el principio de mínimos privilegios, evitando que un proceso tenga más permisos de los necesarios.

Ejemplos Comunes:

    CAP_NET_BIND_SERVICE: Permite abrir puertos menores a 1024 sin ser root.
    CAP_SYS_TIME: Permite ajustar la hora del sistema.
    CAP_SETUID: Permite cambiar el UID del proceso.
    CAP_NET_RAW: Habilita el uso de paquetes en bruto (por ejemplo, ICMP para ping).

Comandos útiles:

    Ver capabilities de un binario:

    bash

getcap /usr/bin/ping

Resultado: /usr/bin/ping = cap_net_raw+ep

Asignar capabilities a un archivo:

bash

sudo setcap cap_net_bind_service=+ep /usr/bin/myapp

Eliminar capabilities:

bash

    sudo setcap -r /usr/bin/myapp

Impacto en Ciberseguridad:

    Escalación de privilegios: Si un binario con setuid tiene malas configuraciones o capacidades elevadas, un atacante puede explotarlo.
    Mitigación: Permite limitar los privilegios de procesos críticos, reduciendo el impacto de compromisos.

Resumen de Capabilities en Windows 🪟

En Windows, las capacidades equivalentes se manejan a través de privilegios y derechos de usuario. Estos determinan lo que un proceso o usuario puede hacer en el sistema. Windows no usa el concepto de setuid, pero proporciona privilegios específicos a través de políticas.
Ejemplos de Privilegios en Windows:

SeBackupPrivilege: Permite leer archivos sin restricciones de permisos (útil para copias de seguridad).
    SeDebugPrivilege: Permite depurar cualquier proceso en el sistema, incluso los que pertenecen a otros usuarios.
    SeTcbPrivilege: Concede al proceso permisos para actuar como parte del sistema operativo (muy peligroso).
    SeShutdownPrivilege: Permite apagar el sistema.

Comandos útiles:

Ver los privilegios de un usuario:

`whoami /priv`

**Agregar un privilegio a un usuario:** (requiere ser administrador)
`ntrights +r SeDebugPrivilege -u usuario
`

#### **Impacto en Ciberseguridad:**

- **Escalación de privilegios:** Si un proceso tiene privilegios como **SeDebugPrivilege**, un atacante podría usarlo para tomar control de otros procesos o escalar privilegios a nivel de sistema.
- **Mitigación:** Implementar **principio de mínimos privilegios** y auditorías frecuentes de los privilegios otorgados a usuarios y servicios.