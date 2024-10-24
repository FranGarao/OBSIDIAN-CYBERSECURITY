## **1. Enumeración de Subdominios**

Estas herramientas son útiles para descubrir subdominios asociados a un dominio principal, lo que es crucial para encontrar APIs ocultas o aplicaciones web adicionales.

### **Subfinder**

- **Resumen**: Subfinder es una herramienta de **enumeración de subdominios pasiva** que utiliza una gran cantidad de fuentes para descubrir subdominios relacionados con un dominio. Es rápida y efectiva, lo que la convierte en una herramienta ideal para comenzar el reconocimiento sin alertar al objetivo.
- **Ejemplo**: `subfinder -d example.com -o subdominios.txt`

### **n0kovo_subdomains**

- **Resumen**: Herramienta rápida para enumerar subdominios utilizando múltiples fuentes de manera eficiente.
- **Ejemplo**: `n0kovo_subdomains -d example.com`

### **OneForAll**

- **Resumen**: Enumerador de subdominios todo-en-uno que utiliza múltiples técnicas y fuentes para encontrar subdominios relacionados.
- **Ejemplo**: `python3 oneforall.py --target example.com run`

### **Subzy**

- **Resumen**: Herramienta para detectar subdominios huérfanos y verificar si pueden ser tomados debido a configuraciones incorrectas.
- **Ejemplo**: `subzy -d example.com`

### **Amass**

- **Resumen**: Amass realiza la enumeración avanzada de subdominios utilizando una combinación de técnicas activas y pasivas.
- **Ejemplo**: `amass enum -d example.com`

### **Assetfinder**

- **Resumen**: Herramienta ligera para la enumeración pasiva de subdominios, obteniendo resultados de varias fuentes en línea.
- **Ejemplo**: `assetfinder --subs-only example.com`

---

## **2. Verificación de Servicios Activos**

Estas herramientas permiten verificar qué subdominios, direcciones IP o hosts tienen servicios HTTP(s) activos.

### **Httpx**

- **Resumen**: Httpx verifica rápidamente los servicios HTTP(s) activos en una lista de dominios o subdominios.
- **Ejemplo**: `httpx -l subdominios.txt -silent`

### **Waybackurls**

- **Resumen**: Extrae todas las URLs históricas de un dominio archivadas en **Wayback Machine** o servicios similares para descubrir rutas antiguas o APIs expuestas.
- **Ejemplo**: `echo "example.com" | waybackurls`

---

## **3. Crawling y Descubrimiento de Endpoints**

Estas herramientas se utilizan para explorar sitios web y APIs, buscando rutas ocultas, endpoints no documentados o parámetros útiles.

### **Katana**

- **Resumen**: Katana realiza crawling en profundidad, identificando endpoints y rutas en aplicaciones web y APIs de forma eficiente.
- **Ejemplo**: `katana -u https://example.com`

### **LinkFinder**

- **Resumen**: Esta herramienta busca rutas o URLs en archivos JavaScript, lo que ayuda a descubrir **endpoints de API** que podrían estar ocultos en el frontend.
- **Ejemplo**: `python3 linkfinder.py -i https://example.com/script.js -o cli`

### **Arjun**

- **Resumen**: Herramienta especializada en descubrir parámetros GET y POST en aplicaciones web y APIs. Ideal para encontrar posibles puntos de inyección de datos.
- **Ejemplo**: `python3 arjun.py -u https://example.com`

---

## **4. Fuzzing de Rutas y Parámetros**

Estas herramientas permiten realizar fuzzing de rutas y parámetros en APIs y aplicaciones web, ayudando a descubrir endpoints ocultos o vulnerabilidades en la entrada de datos.

### **FFUF (Fuzz Faster U Fool)**

- **Resumen**: FFUF es una herramienta extremadamente rápida para realizar fuzzing de rutas, directorios y parámetros.
- **Ejemplo**: `ffuf -u https://example.com/FUZZ -w rutas.txt`

### **Gobuster**

- **Resumen**: Gobuster realiza fuzzing de directorios y subdominios, ayudando a descubrir rutas en APIs y aplicaciones web.
- **Ejemplo**: `gobuster dir -u https://example.com -w rutas.txt`

### **Wfuzz**

- **Resumen**: Herramienta de fuzzing altamente configurable para explorar múltiples parámetros y rutas en APIs. Especialmente útil para probar vulnerabilidades como inyecciones SQL o XSS.
- **Ejemplo**: `wfuzz -c -z file,rutas.txt --hc 404 https://example.com/FUZZ`

---

## **5. Análisis y Detección de Vulnerabilidades**

Estas herramientas están diseñadas para realizar análisis automatizados de vulnerabilidades en APIs y aplicaciones web, cubriendo una amplia gama de pruebas de seguridad.

### **Nuclei**

- **Resumen**: Nuclei permite realizar escaneos de vulnerabilidades usando plantillas predefinidas, ideal para automatizar la búsqueda de problemas de seguridad.
- **Ejemplo**: `nuclei -u https://example.com -t templates/`

### **Nikto**

- **Resumen**: Nikto es un escáner web que busca vulnerabilidades conocidas en servidores web, configuraciones incorrectas y problemas de seguridad básicos.
- **Ejemplo**: `nikto -h https://example.com`

### **OWASP ZAP (Zaproxy)**

- **Resumen**: OWASP ZAP es una herramienta de escaneo y análisis de seguridad que se puede usar para escanear APIs y aplicaciones web, buscando vulnerabilidades como XSS, inyecciones SQL, etc.
- **Ejemplo**: Usar OWASP ZAP en modo proxy para interceptar y analizar el tráfico API.

### **sqlmap**

- **Resumen**: Sqlmap es una herramienta de inyección SQL automatizada que permite detectar y explotar vulnerabilidades SQL en APIs y aplicaciones web.
- **Ejemplo**: `sqlmap -u "https://example.com/api?id=1" --dbs`

---

## **6. Seguridad de Aplicaciones y APIs**

Estas herramientas son más especializadas y te ayudan a descubrir problemas específicos de seguridad en APIs y aplicaciones web, como XSS o rutas vulnerables.

### **XSS Vibes**

- **Resumen**: Herramienta para la detección automática de vulnerabilidades de **Cross-Site Scripting (XSS)** en aplicaciones web que interactúan con el navegador.
- **Ejemplo**: `xss_vibes -u https://example.com -p param`

### **SocialHunter**

- **Resumen**: Herramienta de reconocimiento enfocada en redes sociales, útil para obtener información adicional sobre personas o entidades vinculadas a la administración de una API o aplicación.
- **Ejemplo**: `socialhunter -d example.com`