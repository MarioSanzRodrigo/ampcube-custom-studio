# Privacidad

La web de presentación no incorpora formularios, cuentas, publicidad ni analítica propia. Para mostrar el contador de descargas, tu navegador consulta la API pública de GitHub (recuento de descargas de las releases) y guarda el resultado 10 minutos en su almacenamiento local. Cloudflare, GitHub y Google Fonts (tipografías) pueden procesar los datos técnicos de conexión conforme a sus políticas.

El editor (Windows y Android) funciona en local. Solo se conecta a Internet en estos casos:

- **Pestaña TONE3000:** carga la web de tone3000.com dentro del editor, como un navegador. Si inicias sesión en TONE3000, esa sesión (sus cookies) se guarda solo en tu dispositivo, en los datos del editor; el editor no usa claves de API ni envía tus datos a ningún otro sitio. TONE3000 trata los datos de su web conforme a su propia política.
- **Aviso de versión nueva:** una vez al día, el editor consulta la API pública de GitHub (la última release de este proyecto) para saber si hay una versión más nueva. Es una consulta anónima, sin datos tuyos; GitHub ve la dirección IP como en cualquier visita. Se desactiva en «Acerca de».
- **Descargar la IA del Asistente de tono:** al pulsar «Descargar», el editor baja el modelo de IA Qwen 2.5 desde Hugging Face y, en Windows, también el motor llama.cpp desde GitHub. Son descargas normales de ficheros públicos: no se envía ningún dato tuyo ni se crea ninguna cuenta.

La IA del asistente funciona por completo en tu ordenador o móvil: lo que escribes para describir un sonido no sale del dispositivo. Si en Windows usas Ollama, se le habla solo en tu propio ordenador (127.0.0.1) o en la dirección que tú indiques.

En Windows, el editor usa Microsoft Edge WebView2 con una carpeta de datos propia. Guarda en el dispositivo los ajustes del editor (incluidos el idioma y la fecha de la última comprobación de versión), el último equipo conectado y, si usas TONE3000, su sesión. Las capturas que descargas desde TONE3000 se guardan solo de forma temporal para convertirlas y se borran al cerrar el editor. La IA descargada se guarda en `%LOCALAPPDATA%\AMPCUBE Custom Studio\ai` y el desinstalador la borra. En Android, la IA se guarda en la memoria privada de la app y se borra al desinstalarla.

MIDI (USB o Bluetooth) se usa solo para comunicarse con el AMPCUBE. Las capturas `.nam` se convierten en el propio ordenador o móvil; no se suben a ningún sitio.

El registro MIDI y las copias de seguridad solo se guardan o se comparten por iniciativa del usuario. Antes de compartir un archivo, revisa su contenido.
