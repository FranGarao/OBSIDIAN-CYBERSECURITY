### **SNMP (Simple Network Management Protocol)**

- **Descripción**: Protocolo utilizado para la administración y monitorización de dispositivos de red como routers, switches, servidores y otros dispositivos de red. Proporciona un método para recopilar estadísticas y configurar dispositivos de red.
    
- **Puertos**:
    - **161**: Utilizado para consultas SNMP.
    - **162**: Utilizado para recibir notificaciones SNMP (traps).

- **Seguridad**:
    - **SNMPv3**: Proporciona autenticación y cifrado, a diferencia de las versiones anteriores (SNMPv1 y SNMPv2) que son inseguras.

- **Servicios**:
    - **Net-SNMP** en sistemas Unix/Linux.
    - **Windows SNMP Service** en sistemas Windows.

- **Comandos**:
```
snmpget -v 2c -c public hostname system.sysDescr.0
snmpwalk -v 2c -c public hostname
```