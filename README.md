Faro Morse Interactivo 🏮🔊

Sistema interactivo físico basado en voz para la conversión y emisión de alertas lumínicas en Código Morse mediante Arduino Uno y tecnologías web. Proyecto desarrollado para la Entrega 2 de Diseño de Interfaces (UAI).

🚀 Descripción del Proyecto

El Faro Morse Interactivo permite que una persona dicte una palabra de alerta frente al micrófono del computador (ej. SOS, AYUDA, FUEGO, PELIGRO). La interfaz web procesa la voz utilizando la Web Speech API, la traduce a código Morse y transmite la señal vía Web Serial API a un Arduino Uno conectado físicamente a una tira LED NeoPixel de 8 luces. El faro emite destellos lumínicos en color ámbar siguiendo con precisión la temporización Morse estándar.

🛠️ Tecnologías Utilizadas

Hardware:

Arduino Uno (Controlador central)

Tira LED WS2812 / NeoPixel de 8 luces (Direccionable)

Estructura del faro impresa en 3D (diseño modular cónico)

Cable USB (Transmisión Serial a 9600 baudios y alimentación de 5V)

Software y Librerías:

HTML5 / CSS3 / JavaScript (Panel de control central y simulador)

Web Serial API (Comunicación bidireccional navegador-Arduino)

Web Speech API (Reconocimiento de voz en tiempo real)

Adafruit NeoPixel Library (Gestión de la iluminación en Arduino)

📂 Estructura del Repositorio

📦 Faro-Morse-Interactivo
 ┣ 📂 fotos/
 ┃ ┣ 📜 soldadura.jpg
 ┃ ┣ 📜 fotofaro1.jpg
 ┃ ┣ 📜 fotofaro2.jpg
 ┃ ┣ 📜 fotofaro3.jpg
 ┃ ┣ 📜 video-explicativo.mp4
 ┃ ┗ 📜 Infografía del faro Morse activado por voz.png
 ┣ 📜 index.html              <-- Panel de control maestro, galería y lámina
 ┣ 📜 index-controlador.html  <-- Interfaz de reconocimiento de voz y serial
 ┗ 📜 faro.ino                <-- Firmware para cargar en la placa Arduino Uno


⚙️ Instrucciones de Uso y Configuración

Cargar el Firmware:

Abre el archivo faro.ino en el IDE de Arduino.

Selecciona tu placa Arduino Uno y el puerto COM correspondiente.

Asegúrate de tener instalada la librería Adafruit_NeoPixel e instala el código en la placa.

Ejecutar la Interfaz Web:

Clona o descarga este repositorio en tu computador.

Utiliza una extensión como Live Server (en VS Code) para abrir el archivo index.html.

Conecta el Arduino al puerto USB y haz clic en "Abrir Controlador de Voz" o interactúa desde el panel principal.

Otorga los permisos de micrófono en Google Chrome o Microsoft Edge y comienza a emitir tus alertas de voz.

📸 Registro Fotográfico y Proceso

Manufactura: Soldadura de terminales y cableado a la tira LED.

Prototipado 3D: Modelado modular en secciones (base, cilindros intermedios, cúspide).

Ensamble Final: Integración de la electrónica dentro de la base cónica del faro.
