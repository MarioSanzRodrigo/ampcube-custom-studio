# Licencias, fuentes y créditos

## Editor y app (AMPCUBE Custom Studio)

El editor web, el lanzador de Windows y la app Android (WebView con puente MIDI por
USB y Bluetooth LE) se ofrecen bajo GPL-3.0-only. Las fuentes completas, sin claves de
firma ni rutas locales, van en AMPCUBE-Custom-Studio-3.4-Sources.zip, en la release v4.3.

El conversor de capturas NAM a Clone (nam2clo.js) es código propio. Usa un método de
ajuste multinivel equivalente al de SonicMaster (MIT). Los modelos .nam son del formato
de Neural Amp Modeler (MIT); el editor no incluye ningún modelo.

El editor de Windows incluye las bibliotecas de Microsoft Edge WebView2
(Microsoft.Web.WebView2.Core.dll, Microsoft.Web.WebView2.WinForms.dll y WebView2Loader.dll),
redistribuibles bajo la licencia de Microsoft incluida como LICENSE-WebView2.txt.

La app Android incluye MediaPipe LLM Inference de Google (com.google.mediapipe:tasks-genai),
bajo licencia Apache 2.0 (https://www.apache.org/licenses/LICENSE-2.0), para ejecutar la IA
del Asistente de tono en el móvil.

## IA del Asistente de tono (se descarga aparte, no va en los instaladores)

- Modelos **Qwen 2.5 Instruct** (0,5B y 1,5B) de Alibaba Cloud / equipo Qwen, bajo licencia
  Apache 2.0. En Android, la versión de LiteRT Community (`litert-community` en Hugging Face);
  en Windows, la versión GGUF oficial (`Qwen/Qwen2.5-*-Instruct-GGUF`).
- Motor **llama.cpp** (ggml-org), bajo licencia MIT, versión b12292 para Windows x64 con Vulkan,
  descargado de su release oficial en GitHub.

El editor comprueba el SHA-256 de cada descarga en Windows antes de usarla.

La pestaña TONE3000 muestra la web pública de tone3000.com. Las capturas que se
descargan desde ella pertenecen a sus autores y conservan su licencia; el editor no
incluye ni redistribuye ninguna.

## AMPCUBE Custom Firmware

El archivo de firmware es una versión modificada del firmware oficial V1.2.3 de
Sonicake para el AMPCUBE. Contiene el código y los datos originales de Sonicake, a los
que se añaden parches propios en el procesador principal y el DSP. Los amplificadores y
delays añadidos proceden de la custom del PocketMaster, de la misma plataforma.
Los derechos sobre el firmware original pertenecen a Sonicake. Este proyecto es
independiente y no está afiliado, patrocinado ni aprobado por Sonicake.

El firmware se distribuye tal cual, sin garantía de ningún tipo. Instalarlo es
responsabilidad de cada usuario. Se puede volver en cualquier momento al firmware
oficial con Sonicake Manager.

## Marcas

SONICAKE, AMPCUBE, Pocket Master y TONE3000 son marcas de sus titulares. Se citan para identificar
los dispositivos compatibles; no implican patrocinio ni aprobación. Los dibujos de esta
web son representaciones propias. Los nombres de los modelos son los que usa el propio
firmware.
