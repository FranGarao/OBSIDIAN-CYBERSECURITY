### **NTP (Network Time Protocol)**

- **Descripción**: Protocolo utilizado para sincronizar la hora entre dispositivos en una red.
    
- **Puertos**:
    - **123** por defecto (UDP).
    
- **Seguridad**: NTP no cifra las comunicaciones. Versiones más recientes soportan autenticación, pero aún pueden ser vulnerables a ciertos ataques (como NTP amplification).

- **Servicios**:
    - **ntpd (NTP daemon)**
    - **Chrony**
    
- **Comandos**:
```
ntpdate -q pool.ntp.org
timedatectl status
```