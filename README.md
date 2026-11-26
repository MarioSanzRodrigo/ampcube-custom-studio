# AMPCUBE Custom Firmware by Dokken · AMPCUBE Custom Studio

Firmware custom, editor de escritorio y app Android para **Sonicake AMPCUBE**, por [Dokken](https://guitarristas.info/usuarios/dokken7789).

**[Web y descargas](https://ampcube-custom-studio.pages.dev/)** · [Wiki](https://ampcube-custom-studio.pages.dev/wiki.html) · [Release v4.1](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/tag/v4.1)

| | Versión | Descarga |
|---|---|---|
| AMPCUBE Custom Firmware | v4 (base oficial V1.2.3) | [AMPCUBE_V1.2.3_CustomFW_v4.bin](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v4.1/AMPCUBE_V1.2.3_CustomFW_v4.bin) |
| AMPCUBE Custom Studio para Android | 3.1 · Android 8+ · Bluetooth o USB OTG | [APK](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v4.1/AMPCUBE-Custom-Studio-3.1-Android.apk) · [Fuentes](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v4.1/AMPCUBE-Custom-Studio-3.1-Sources.zip) |
| AMPCUBE Custom Studio para Windows | 3.1 · Windows 10/11 | [Instalador](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v4.1/AMPCUBE-Custom-Studio-3.1-Setup.exe) |

## Firmware

- **13 huecos NAM** (de serie, 5).
- **Low Cut y High Cut en el bloque IR:** de 20 Hz a 20 kHz, en tiempo real, también con NAM + IR.
- **NAM y cabina a la vez:** la IR suena detrás de la captura NAM (convolución por software de 512 taps), con su VOL.
- **37 amplificadores** (de serie, 21): 15 de la custom del PocketMaster y el Brit 900, que el Manager oficial ocultaba.
- **17 delays** (de serie, 8): Echo, Shiny, Dark, Float, Damage, Flash, Shake, Glost y Flutter.
- Mantiene los 5 huecos de IR de usuario y las 15 cabinas de fábrica.
- **Seguridad:** si algo falla, enciende el equipo con la perilla PARA pulsada y flashea el oficial con Sonicake Manager.

Instrucciones y notas en `FIRMWARE-v4.md`, dentro de la release.

## Editor (Windows y Android)

- **Asistente de tono:** describes el sonido (un grupo, una canción, un guitarrista o un estilo) y crea un preset solo con los modelos del AMPCUBE, sin NAM ni IR de usuario. Lo carga en el equipo sin guardarlo para que lo pruebes y retoques, y lo guardas donde quieras.
  - **IA integrada opcional, sin cuentas ni claves:** en el móvil o en el PC se descarga una vez un modelo Qwen 2.5 y funciona sin Internet. Puedes pedir una versión B a la IA y compararla con la A, con el volumen igualado.
- **TONE3000 integrado:** la web de TONE3000 se abre dentro del editor. Al descargar una captura, el editor la convierte al formato Clone y la carga en el hueco que elijas.
- **Métricas NAM vs CLONE:** tras convertir una captura verás su fidelidad, el error y la relación señal/error por intensidad, la diferencia de volumen y la respuesta en frecuencia de los dos.
- **Low Cut y High Cut** en Hz en el bloque IR, con un botón para activarlos y desactivarlos y comparar.
- **Funciones:**
  - biblioteca de presets de usuario y de fábrica, con búsqueda y renombrado;
  - cadena de señal: encender, apagar y reordenar bloques;
  - perillas en vivo (en el móvil, deslizadores grandes) y guardado con aviso de cambios pendientes;
  - huecos de IR y NAM: subir, renombrar y vaciar;
  - conversión directa de capturas `.nam` (A1 y A2, WaveNet y LSTM);
  - ajustes globales y copias de seguridad.
- **Windows:** se instala en tu usuario, sin permisos de administrador, y se abre en su propia ventana (Microsoft Edge WebView2). Conexión por USB.
- **Android:** conexión por Bluetooth (BLE MIDI), sin emparejar antes, o por cable con USB OTG. Interfaz pensada para el móvil.

Cierra Sonicake Manager y la app oficial antes de conectar. Los instaladores no llevan firma digital comercial.

## Repositorio

- **Documentación:** este repositorio solo la contiene.
- **Código:** el código completo del editor y de la app va en `Sources.zip`, dentro de cada release. El «Source code» automático de GitHub solo contiene este árbol de documentación.
- **Licencias:**
  - el editor y la app están bajo GPL-3.0-only;
  - el firmware es una modificación del firmware oficial de Sonicake, cuyos derechos pertenecen a Sonicake.

Proyecto independiente, sin vinculación oficial con Sonicake ni con TONE3000. Sin garantía: lo instalas bajo tu responsabilidad.
