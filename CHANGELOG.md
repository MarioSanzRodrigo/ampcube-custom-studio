# Cambios

## v2.0.2 · AMPCUBE Custom Studio 1.5

El firmware no cambia: sigue siendo la v2.

- **Pantalla de conexión nueva:** un AMPCUBE animado (el cono respira, los LEDs laten, salen ondas) con solo Conectar y Demo. Mientras conecta muestra «Buscando tu AMPCUBE…» o «Conectando…» y un botón Cancelar. Una sola conexión a la vez.
- **Conexión mucho más rápida:** el editor se puede usar en cuanto lee el preset actual. Nombres, listas de IR y NAM y ajustes salen de la última conexión y se actualizan en segundo plano («Conectado · actualizando datos…»). Por Bluetooth, en pruebas con un equipo simulado lento: de 14,6 s a 3,0 s.
- **Cambio de preset fluido:** un preset ya visitado aparece al instante; uno nuevo se atenúa hasta que llega. Con varias pulsaciones seguidas solo se carga el último.
- **Menos tráfico por Bluetooth:** la relectura completa del preset es cada 10 s y se para mientras cambias de preset.
- Ya no aparece «El AMPCUBE se ha desconectado» al pulsar Desconectar o Cancelar.

## v2.0.1 · AMPCUBE Custom Studio 1.4.1

El firmware no cambia: sigue siendo la v2.

- **Modelos nuevos:** los amplis y delays del firmware custom llevan la etiqueta «Custom FW v2» y «Portado de la custom del PocketMaster», en lugar de «AMPCUBE de serie».
- **NAM + IR:** con el firmware custom, el bloque AMP en modo NAM indica que la IR suena detrás de la captura y ofrece «Encender IR junto al NAM» si el bloque IR está apagado. Ya no aparece como experimental.
- **Firmware oficial:** el editor explica que con el firmware oficial el NAM sustituye al AMP y a la IR, y no ofrece encender la IR con el NAM.
- «Acerca de» muestra el nombre y la versión del editor.

## v2.0 · AMPCUBE Custom Firmware v2 + AMPCUBE Custom Studio 1.4

Primera versión pública.

### Firmware v2 (Sonicake AMPCUBE, base oficial V1.2.3)

- **NAM y cabina a la vez:** convolución IR por software de 512 taps mientras el bloque Clone (NAM) está activo, con el VOL del IR.
- **10 huecos NAM** (de serie, 5).
- **16 amplificadores más (37):** 15 portados de la custom del PocketMaster y el Brit 900 de serie, que el Manager oficial ocultaba.
- **9 delays más (17):** Echo, Shiny, Dark, Float, Damage, Flash, Shake, Glost y Flutter.

### AMPCUBE Custom Studio 1.4 (Windows y Android)

- Reconoce el firmware custom y muestra sus amplis, delays y 10 huecos NAM.
- Conversión directa de capturas `.nam` al formato Clone del AMPCUBE (WaveNet estándar, lite, feather, nano, NAM 0.7 y LSTM), también sin el equipo conectado.
- Biblioteca de presets, cadena con reordenado, perillas en vivo, guardado con aviso de cambios, huecos de IR y NAM, ajustes globales y copias.
- Android: Bluetooth (BLE MIDI) o USB OTG.
- Los desplegables ya no se cierran solos mientras el editor sincroniza con el equipo.
