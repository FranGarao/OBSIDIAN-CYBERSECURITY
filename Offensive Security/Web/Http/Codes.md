### **1xx - Respuestas informativas**

Indican que la solicitud ha sido recibida y el servidor está en proceso de realizarla. En ciberseguridad ofensiva, los 1xx son menos comunes, pero pueden ser útiles durante ataques de reconocimiento.

- **100**: Continue – El cliente puede continuar con la solicitud.
- **101**: Switching Protocols – El servidor está cambiando el protocolo según la solicitud del cliente.
- **102**: Processing – Indica que el servidor ha recibido y está procesando la solicitud, pero aún no ha finalizado (WebDAV).
- **103**: Early Hints – Permite enviar encabezados preliminares antes de la respuesta final.

### **2xx - Respuestas satisfactorias**

Indican que la solicitud ha sido recibida, comprendida y aceptada con éxito.

- **200**: OK – La solicitud se ha completado correctamente.
- **201**: Created – Un nuevo recurso ha sido creado como resultado de la solicitud.
- **202**: Accepted – La solicitud ha sido aceptada, pero el procesamiento aún no ha sido completado.
- **203**: Non-Authoritative Information – El servidor ha devuelto información modificada.
- **204**: No Content – La solicitud se ha completado, pero no hay contenido para enviar.
- **205**: Reset Content – Solicita al cliente que reinicie la vista del documento.
- **206**: Partial Content – Respuesta parcial a una solicitud de un recurso específico (usualmente para **ataques de enumeración** cuando se obtiene un recurso por partes).
- **207**: Multi-Status – Devuelve múltiples estados (WebDAV).
- **208**: Already Reported – Se informa de que el recurso ya fue enumerado (WebDAV).
- **226**: IM Used – El servidor ha cumplido una solicitud GET para el recurso y ha utilizado una transformación delta.

### **3xx - Redirecciones**

Indican que se necesita una acción adicional por parte del cliente para completar la solicitud. En **ataques de redirección** o **enumeración**, los códigos 3xx son útiles para detectar configuraciones erróneas o encontrar recursos ocultos.

- **300**: Multiple Choices – Hay varias opciones para el recurso solicitado.
- **301**: Moved Permanently – El recurso solicitado ha sido movido permanentemente a una nueva URL.
- **302**: Found – El recurso solicitado reside temporalmente en una URI diferente.
- **303**: See Other – El servidor está indicando al cliente que consulte otra URI.
- **304**: Not Modified – El recurso no ha sido modificado desde la última solicitud, útil en **cache-poisoning**.
- **305**: Use Proxy – Se debe acceder al recurso solicitado a través de un proxy (obsoleto en la práctica moderna, pero aún presente).
- **307**: Temporary Redirect – El recurso solicitado ha sido movido temporalmente.
- **308**: Permanent Redirect – El recurso solicitado ha sido movido permanentemente (similar a 301).

### **4xx - Errores del cliente**

Son los más utilizados en pruebas de penetración, ya que indican problemas de validación, autenticación o permisos. Los códigos 4xx son claves para explotar errores de autenticación, **ataques de fuerza bruta**, y **SQL injection**.

- **400**: Bad Request – La solicitud no puede ser procesada debido a sintaxis incorrecta.
- **401**: Unauthorized – Se requiere autenticación para acceder al recurso (clave en ataques de fuerza bruta o bypass de autenticación).
- **402**: Payment Required – Reservado para uso futuro (raramente usado).
- **403**: Forbidden – El servidor entiende la solicitud, pero se niega a cumplirla. Útil para detectar **filtros de permisos**.
- **404**: Not Found – El recurso solicitado no existe, usado en **fuzzing de directorios**.
- **405**: Method Not Allowed – El método de solicitud no está permitido para el recurso. Útil para detectar **métodos HTTP no restringidos** como PUT o DELETE.
- **406**: Not Acceptable – No se puede responder en un formato aceptable para el cliente.
- **407**: Proxy Authentication Required – Similar a 401, pero para proxies.
- **408**: Request Timeout – La solicitud ha excedido el tiempo de espera del servidor.
- **409**: Conflict – El recurso está en conflicto con el estado actual del servidor (utilizado en contextos de edición simultánea).
- **410**: Gone – El recurso ya no está disponible y no se proporcionará una nueva URL.
- **411**: Length Required – Se requiere una longitud de contenido válida para completar la solicitud.
- **412**: Precondition Failed – Falló una precondición en los encabezados de la solicitud.
- **413**: Payload Too Large – La solicitud es demasiado grande para ser procesada.
- **414**: URI Too Long – El URI proporcionado es demasiado largo (usado en ataques de **DoS basado en URI largos**).
- **415**: Unsupported Media Type – El servidor no admite el formato del cuerpo de la solicitud.
- **416**: Range Not Satisfiable – El servidor no puede servir la parte solicitada del recurso.
- **417**: Expectation Failed – El servidor no puede cumplir con los requisitos del encabezado Expect.
- **418**: I'm a teapot – Código de broma definido en el RFC 2324 (Hyper Text Coffee Pot Control Protocol), no usado en ciberseguridad.
- **421**: Misdirected Request – La solicitud fue enviada a un servidor que no puede responder.
- **422**: Unprocessable Entity – El servidor entiende la solicitud, pero no puede procesarla (WebDAV, útil en análisis de APIs vulnerables).
- **423**: Locked – El recurso está bloqueado (WebDAV).
- **424**: Failed Dependency – Una solicitud falló debido a la falla de una solicitud anterior (WebDAV).
- **425**: Too Early – Indica que el servidor no está dispuesto a procesar la solicitud (usado para evitar repetición prematura).
- **426**: Upgrade Required – El cliente debe cambiar a otro protocolo (útil para explotar vulnerabilidades en la actualización de protocolos).
- **428**: Precondition Required – El servidor requiere que la solicitud cumpla con una precondición.
- **429**: Too Many Requests – El cliente ha enviado demasiadas solicitudes en un corto periodo (útil para detectar limitación de tasa en **ataques de fuerza bruta**).
- **431**: Request Header Fields Too Large – Los campos de encabezado de la solicitud son demasiado grandes.
- **451**: Unavailable For Legal Reasons – El recurso no está disponible por razones legales (útil en reconocimiento de restricciones geográficas o censura).

### **5xx - Errores del servidor**

Indican que el servidor ha encontrado un problema. Son críticos en **ataques de denegación de servicio (DoS)**, **RCE** y detección de fallos de configuración del servidor.

- **500**: Internal Server Error – El servidor ha encontrado un error inesperado.
- **501**: Not Implemented – El servidor no tiene la funcionalidad para procesar la solicitud.
- **502**: Bad Gateway – El servidor, actuando como gateway o proxy, recibió una respuesta inválida del servidor ascendente.
- **503**: Service Unavailable – El servidor no está disponible temporalmente (útil en ataques de saturación o **DoS**).
- **504**: Gateway Timeout – El servidor, actuando como gateway o proxy, no ha recibido respuesta a tiempo.
- **505**: HTTP Version Not Supported – El servidor no soporta la versión del protocolo HTTP usada en la solicitud.
- **506**: Variant Also Negotiates – Un error de configuración de contenido negociable.
- **507**: Insufficient Storage – El servidor no puede almacenar la representación requerida (WebDAV).
- **508**: Loop Detected – Un loop fue detectado en el procesamiento de la solicitud (WebDAV).
- **510**: Not Extended – Se requiere más extensión en la solicitud.
- **511**: Network Authentication Required – Se requiere autenticación de red para acceder al recurso.

### Códigos adicionales en contextos específicos (usualmente no estándar):

- **598**: Network Read Timeout Error – Un error en la lectura de la red.
- **599**: Network Connect Timeout Error – Un error en la conexión de red.

### **Códigos importantes en ciberseguridad ofensiva**:

1. **401 Unauthorized**: Ideal para identificar sistemas vulnerables a **ataques de fuerza bruta**.
2. **403 Forbidden**: Utilizado para detectar **bypass de acceso** a recursos restringidos.
3. **404 Not Found**: Crucial para el **fuzzing de rutas y directorios**.
4. **500 Internal Server Error**: A menudo indicativo de **inyección de código** o mal manejo de excepciones en el servidor.
5. **503 Service Unavailable**: Usado en **ataques de denegación de servicio (DoS)** para medir el impacto.