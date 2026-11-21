# AMPCUBE Custom Firmware by Dokken · AMPCUBE Custom Studio

Firmware custom, editor de escritorio y app Android para **Sonicake AMPCUBE**, por [Dokken](https://guitarristas.info/usuarios/dokken7789).

**[Web y descargas](https://ampcube-custom-studio.pages.dev/)** · [Release v2.0](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/tag/v2.0)

| | Versión | Descarga |
|---|---|---|
| AMPCUBE Custom Firmware | v2 (base oficial V1.2.3) | [AMPCUBE_V1.2.3_CustomFW_v2.bin](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v2.0/AMPCUBE_V1.2.3_CustomFW_v2.bin) |
| AMPCUBE Custom Studio para Android | 1.4 · Android 8+ · Bluetooth o USB OTG | [APK](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v2.0/AMPCUBE-Custom-Studio-1.4-Android.apk) · [Fuentes](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v2.0/AMPCUBE-Custom-Studio-1.4-Sources.zip) |
| AMPCUBE Custom Studio para Windows | 1.4 · Windows 10/11 | [Instalador](https://github.com/MarioSanzRodrigo/ampcube-custom-studio/releases/download/v2.0/AMPCUBE-Custom-Studio-1.4-Setup.exe) |

## Firmware

- **NAM y cabina a la vez:** la IR suena detrás de la captura NAM (convolución por software de 512 taps), con su VOL.
- **10 huecos NAM** (de serie, 5).
- **37 amplificadores** (de serie, 21): 15 de la custom del PocketMaster y el Brit 900, que el Manager oficial ocultaba.
- **17 delays** (de serie, 8): Echo, Shiny, Dark, Float, Damage, Flash, Shake, Glost y Flutter.
- Mantiene los 5 huecos de IR de usuario y las 15 cabinas de fábrica.
- **Seguridad:** si algo falla, enciende el equipo con la perilla PARA pulsada y flashea el oficial con Sonicake Manager.

Instrucciones y notas en `FIRMWARE-v2.md`, dentro de la release.

## Editor (Windows y Android)

- **Funciones:**
  - biblioteca de presets de usuario y de fábrica, con búsqueda y renombrado;
  - cadena de señal: encender, apagar y reordenar bloques;
  - perillas en vivo y guardado con aviso de cambios pendientes;
  - huecos de IR y NAM: subir, renombrar y vaciar;
  - conversión directa de capturas `.nam` (WaveNet y LSTM) al formato del AMPCUBE, con fidelidad estimada;
  - ajustes globales y copias de seguridad.
- **Windows:** se instala en tu usuario, sin permisos de administrador, y se abre en su propia ventana. Conexión por USB.
- **Android:** conexión por Bluetooth (BLE MIDI), sin emparejar antes, o por cable con USB OTG.

Cierra Sonicake Manager y la app oficial antes de conectar. Los instaladores no llevan firma digital comercial.

## Repositorio

- **Documentación:** este repositorio solo la contiene.
- **Código:** el código completo del editor y de la app va en `Sources.zip`, dentro de cada release. El «Source code» automático de GitHub solo contiene este árbol de documentación.
- **Licencias:**
  - el editor y la app están bajo GPL-3.0-only;
  - el firmware es una modificación del firmware oficial de Sonicake, cuyos derechos pertenecen a Sonicake.

Proyecto independiente, sin vinculación oficial con Sonicake. Sin garantía: lo instalas bajo tu responsabilidad.
