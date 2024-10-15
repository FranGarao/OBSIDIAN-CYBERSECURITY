### **Comandos básicos del sistema**

1. **ls** – Lista el contenido del directorio actual.
2. **cd** – Cambia de directorio.
3. **pwd** – Muestra la ruta del directorio actual.
4. **mkdir** – Crea un nuevo directorio.
5. **rmdir** – Elimina un directorio vacío.
6. **rm** – Elimina archivos o directorios.
7. **cp** – Copia archivos o directorios.
8. **mv** – Mueve o renombra archivos y directorios.
9. **touch** – Crea archivos vacíos.
10. **find** – Busca archivos en directorios.
11. **locate** – Encuentra archivos rápidamente usando índices.
12. **updatedb** – Actualiza la base de datos para `locate`.
13. **tree** – Muestra la estructura de directorios en forma de árbol.
14. **stat** – Muestra detalles de un archivo.
15. **file** – Identifica el tipo de un archivo.
16. **df** – Muestra el espacio libre en disco.
17. **du** – Muestra el uso de espacio en directorios.
18. **ln** – Crea enlaces simbólicos o duros.
19. **alias** – Define alias para comandos.
20. **unalias** – Elimina alias.
21.  **which** - Muestra la ruta del binario ejecutable si está en tu `PATH`.
22. **whereis** -  Busca binarios, fuentes y archivos de manual relacionados con el programa.
23. **type** - Verifica si el comando es un alias, función o binario.
24. **command** - Muestra la ruta del comando si está en el `PATH`.
25. **dpkg** - Busca si un paquete específico está instalado.

---

### **Comandos de gestión de procesos y rendimiento**

21. **ps** – Muestra los procesos en ejecución.
22. **top** – Muestra los procesos más activos en tiempo real.
23. **htop** – Interfaz mejorada de `top` (debe instalarse).
24. **kill** – Termina un proceso por su PID.
25. **pkill** – Termina procesos por nombre.
26. **xkill** – Cierra ventanas gráficamente.
27. **jobs** – Lista procesos en segundo plano.
28. **bg** – Restaura un proceso en segundo plano.
29. **fg** – Trae un proceso al primer plano.
30. **nice** – Ejecuta un comando con prioridad modificada.
31. **renice** – Cambia la prioridad de un proceso en ejecución.

---

### **Comandos de usuario y permisos**

32. **whoami** – Muestra el nombre del usuario actual.
33. **id** – Muestra información del usuario y grupos.
34. **who** – Muestra quién está conectado al sistema.
35. **w** – Muestra qué hacen los usuarios conectados.
36. **groups** – Muestra los grupos a los que pertenece el usuario.
37. **chmod** – Cambia permisos de archivos.
38. **chown** – Cambia el propietario de un archivo.
39. **usermod** – Modifica cuentas de usuario.
40. **useradd** – Crea nuevos usuarios.
41. **userdel** – Elimina usuarios.
42. **passwd** – Cambia contraseñas de usuarios.
43. **sudo** – Ejecuta comandos con permisos de superusuario.

---

### **Comandos de red y conectividad**

44. **ping** – Comprueba la conectividad con otra máquina.
45. **ifconfig** – Configura interfaces de red (obsoleto, reemplazado por `ip`).
46. **ip** – Muestra y gestiona configuración de red.
47. **netstat** – Muestra conexiones de red activas.
48. **ss** – Muestra conexiones de red detalladas (reemplaza a `netstat`).
49. **traceroute** – Muestra la ruta a una dirección IP.
50. **nslookup** – Consulta servidores DNS.
51. **dig** – Realiza consultas DNS avanzadas.
52. **curl** – Realiza peticiones HTTP.
53. **wget** – Descarga archivos desde la web.
54. **scp** – Copia archivos entre máquinas vía SSH.
55. **sftp** – Transfiere archivos vía SSH.
56. **ftp** – Cliente para transferencias FTP.
57. **ssh** – Conecta a servidores de forma segura.
58. **telnet** – Cliente para conexiones a servidores.
59. **netcat (nc)** – Herramienta para análisis de red y shells reversos.
60. **socat** – Redirección avanzada de puertos.
61. **tcpdump** – Captura tráfico de red para análisis.
62. **wireshark** – Análisis avanzado de tráfico de red.

---

### **Comandos de archivo y texto**

63. **cat** – Muestra el contenido de archivos.
64. **tac** – Muestra el contenido de archivos al revés.
65. **more** – Muestra archivos de texto por páginas.
66. **less** – Similar a `more`, pero más funcional.
67. **head** – Muestra las primeras líneas de un archivo.
68. **tail** – Muestra las últimas líneas de un archivo.
69. **nl** – Muestra archivos con líneas numeradas.
70. **wc** – Cuenta líneas, palabras y caracteres.
71. **sort** – Ordena líneas de un archivo.
72. **uniq** – Elimina líneas duplicadas.
73. **cut** – Extrae secciones de líneas.
74. **paste** – Une archivos línea por línea.
75. **grep** – Busca patrones en archivos.
76. **awk** – Procesa y analiza texto.
77. **sed** – Edita texto de forma automática.
78. **diff** – Compara archivos línea por línea.
79. **cmp** – Compara archivos byte por byte.

---

### **Compresión y empaquetado**

80. **tar** – Empaqueta múltiples archivos en uno solo.
81. **gzip** – Comprime archivos.
82. **gunzip** – Descomprime archivos gzip.
83. **bzip2** – Comprime archivos con bzip2.
84. **bunzip2** – Descomprime archivos bzip2.
85. **zip** – Crea archivos zip.
86. **unzip** – Extrae archivos zip.

---

### **Comandos del sistema y logs**

87. **dmesg** – Muestra mensajes del kernel.
88. **uptime** – Muestra cuánto tiempo lleva encendida la máquina.
89. **hostname** – Muestra o cambia el nombre del sistema.
90. **uname** – Muestra información del sistema operativo.
91. **vmstat** – Muestra estadísticas del sistema.
92. **iostat** – Muestra estadísticas de entrada/salida.
93. **free** – Muestra el uso de memoria.
94. **lsof** – Lista archivos abiertos.
95. **mount** – Monta sistemas de archivos.
96. **umount** – Desmonta sistemas de archivos.
97. **fsck** – Verifica y repara sistemas de archivos.
98. **shutdown** – Apaga el sistema.
99. **reboot** – Reinicia el sistema.
100. **systemctl** – Controla el estado de servicios.
101. **journalctl** – Muestra logs del sistema.

---

### **Comandos avanzados para hacking**

102. **hydra** – Fuerza bruta contra servicios de red.
103. **john** – Crackeo de contraseñas.
104. **hashcat** – Crackeo avanzado de hashes.
105. **msfconsole** – Inicia el framework de Metasploit.
106. **searchsploit** – Busca exploits en la base de datos.
107. **sqlmap** – Automatiza inyecciones SQL.
108. **nikto** – Escanea vulnerabilidades en servidores web.
109. **gobuster** – Fuerza bruta en directorios web.
110. **dirb** – Escanea directorios ocultos.
111. **Responder** – Captura hashes en redes SMB.
112. **BloodHound** – Mapea Active Directory.
113. **Impacket** – Herramientas para redes Windows.
114. **CrackMapExec** – Automatiza ataques en redes.
115. **nishang** – Scripts PowerShell para explotación.
116. **Burp Suite** – Proxy para analizar tráfico HTTP.
117. **enum4linux** – Enumeración SMB en Linux/Windows.
118. **LinPEAS/WinPEAS** – Escalación de privilegios.
119. **theHarvester** – Recopila información de objetivos.
120. **Ffuf** – Fuerza bruta en directorios y archivos.


---
### **Complementos para hacking y pentesting**

121. **ncat** – Variante de Netcat, incluida en Nmap, con soporte para TLS.
122. **powershell** – Interpreta scripts de PowerShell para manipulación avanzada en Windows.
123. **zmap** – Escanea puertos masivamente en redes a gran escala.
124. **amass** – Herramienta avanzada para descubrimiento de subdominios.
125. **sslscan** – Escanea servidores para detectar configuraciones SSL/TLS débiles.
126. **feroxbuster** – Fuerza bruta rápida para descubrir directorios ocultos en aplicaciones web (similar a Gobuster).
127. **cewl** – Genera diccionarios personalizados a partir de páginas web.
128. **wpscan** – Escanea sitios de WordPress en busca de vulnerabilidades conocidas.
129. **medusa** – Alternativa a Hydra para ataques de fuerza bruta.
130. **msfvenom** – Genera payloads personalizados para Metasploit.

---

### **Comandos útiles en análisis forense**

131. **foremost** – Extrae archivos eliminados o corruptos de imágenes de disco.
132. **photorec** – Recupera archivos borrados desde medios dañados o corruptos.
133. **autopsy** – Interfaz gráfica para análisis forense de discos.
134. **volatility** – Framework para análisis de memoria RAM.

---

### **Comandos adicionales de automatización y programación**

135. **tmux** – Multiplexor de terminal para gestionar múltiples sesiones.
136. **screen** – Permite mantener sesiones de terminal activas en segundo plano.
137. **expect** – Automatiza interacciones con otros programas en la línea de comandos.
138. **ansible** – Automatiza tareas y configuraciones en múltiples servidores.

---

### **Comandos adicionales de monitoreo y logs**

139. **strace** – Muestra las llamadas al sistema realizadas por un proceso.
140. **ltrace** – Muestra las llamadas a funciones de bibliotecas dinámicas.
141. **tcpflow** – Captura tráfico TCP y lo muestra en formato legible.
142. **ngrep** – Similar a grep, pero para tráfico de red.

---

### **Comandos de criptografía y análisis de hashes**

143. **openssl** – Genera y verifica certificados, y realiza operaciones criptográficas.
144. **gpg** – Cifra y firma archivos con criptografía de clave pública.
145. **base64** – Codifica y decodifica datos en Base64.
146. **sha256sum** – Genera hashes SHA-256 para verificar integridad de archivos.

---

### **Comandos para manipulación de imágenes y binarios**

147. **xxd** – Muestra contenido de archivos en hexadecimal (útil en ingeniería inversa).
148. **binwalk** – Analiza binarios en busca de datos ocultos o incrustados.
149. **radare2** – Framework para análisis de binarios y exploit development.

---

### **Comandos adicionales para control y explotación en redes**

150. **ettercap** – Herramienta para ataques MITM (Man-in-the-Middle).
151. **aircrack-ng** – Suite para crackeo de redes Wi-Fi.
152. **reaver** – Ataque a redes Wi-Fi usando vulnerabilidades WPS.
153. **wifite** – Automatiza ataques a redes inalámbricas.

---

### **Otros comandos avanzados para pentesting**

154. **dnsenum** – Enumeración avanzada de DNS.
155. **cewl** – Extrae palabras clave para crear diccionarios personalizados.
156. **proxychains** – Encadena proxies para ocultar la IP durante conexiones.
157. **torsocks** – Ejecuta comandos a través de la red Tor.
158. **beeF** – Framework para explotación de navegadores.
---

### **Comandos adicionales para captura y análisis de tráfico**

159. **tshark** – Versión de línea de comandos de Wireshark para capturar y analizar tráfico.
160. **tcpick** – Captura y analiza sesiones TCP (útil para reconstruir flujos de datos).
161. **ngrep** – Similar a `grep`, pero para buscar patrones en tráfico de red en vivo.
162. **netsniff-ng** – Suite avanzada para sniffing y análisis de tráfico en redes.
163. **dnsspoof** – Captura y manipula tráfico DNS.
164. **bettercap** – Framework avanzado para ataques MITM y análisis en redes.

---

### **Comandos de explotación avanzada y herramientas de payloads**

165. **empire** – Framework de post-explotación basado en PowerShell y Python.
166. **cobalt strike** – Plataforma de red teaming y explotación avanzada.
167. **msfvenom** – Genera payloads personalizados para Metasploit (útil para shells reversos).
168. **veil** – Generador de payloads que evade antivirus.
169. **fatrat** – Crea backdoors con capacidad de evasión de antivirus.

---

### **Comandos para hacking de redes inalámbricas**

170. **airodump-ng** – Escanea y captura tráfico en redes inalámbricas.
171. **aireplay-ng** – Inyecta paquetes en redes Wi-Fi para ataques de desautenticación.
172. **airmon-ng** – Habilita modo monitor en interfaces de red inalámbrica.
173. **wifite** – Automatiza ataques a redes Wi-Fi, combinando herramientas de Aircrack.

---

### **Comandos para manipulación de binarios y analisis de malware**

174. **gdb** – Depurador para programas en sistemas Linux (útil en ingeniería inversa).
175. **objdump** – Muestra información de binarios ejecutables.
176. **readelf** – Extrae información de archivos ELF en sistemas Linux.
177. **radare2** – Framework de ingeniería inversa y explotación.
178. **strace** – Traza las llamadas al sistema realizadas por un programa.
179. **ltrace** – Traza las llamadas a bibliotecas dinámicas.
180. **pwntools** – Framework para explotación y CTFs en Python.

---

### **Comandos para evasión y anonimato**

181. **proxychains** – Encadena proxies para ocultar la IP en conexiones.
182. **torsocks** – Redirige conexiones a través de la red Tor.
183. **openvpn** – Conecta a redes privadas mediante VPN.
184. **iptables** – Configura reglas de firewall para gestionar tráfico entrante y saliente.

---

### **Comandos de descubrimiento y enumeración de servicios**

185. **dnsrecon** – Enumeración de registros DNS.
186. **dnsenum** – Descubre registros DNS y subdominios.
187. **snmpwalk** – Recupera información SNMP de dispositivos de red.
188. **enum4linux** – Enumeración de recursos compartidos en redes Windows SMB.
189. **theHarvester** – Recopila correos electrónicos, subdominios y usuarios a partir de fuentes públicas.
190. **amass** – Descubrimiento masivo de subdominios y mapeo de infraestructura.

---

### **Comandos adicionales para automatización y gestión de sesiones**

191. **tmux** – Multiplexor de terminal para gestionar múltiples sesiones.
192. **screen** – Permite mantener sesiones persistentes en segundo plano.
193. **expect** – Automatiza interacciones con otros programas en la línea de comandos.
194. **ansible** – Automatiza configuraciones y tareas en múltiples servidores.

---

### **Criptografía y generación de certificados**

195. **openssl** – Realiza operaciones criptográficas y genera certificados.
196. **gpg** – Cifra y firma datos con criptografía de clave pública.
197. **certbot** – Automatiza la generación y renovación de certificados SSL con Let's Encrypt.
198. **hashid** – Identifica tipos de hashes para facilitar su crackeo.
199. **base64** – Codifica y decodifica datos en Base64.
200. **sha256sum** – Genera y verifica hashes SHA-256.
