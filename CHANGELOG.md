# Cambios

## v4.1 · AMPCUBE Custom Studio 3.1

El firmware no cambia: sigue siendo la v4.

- **Low Cut y High Cut del IR:** los fijas con las perillas, sin valores por defecto. El botón **Apagar filtros** los pone en Off guardando tus valores y **Encender filtros** los devuelve tal cual, para comparar mientras tocas. Si mueves una perilla con los filtros apagados, se vuelven a encender.
- **IR y NAM:** los huecos vacíos se ven otra vez como una fila normal («vacío») en lugar de un recuadro grande.

## v4.0 · AMPCUBE Custom Firmware v4 + AMPCUBE Custom Studio 3.0

### Firmware v4 (base oficial V1.2.3)

- **13 huecos NAM** (en la v2, 10; de serie, 5).
- **Low Cut y High Cut en el bloque IR**, de 20 Hz a 20 kHz y en tiempo real (filtros de 12 dB/oct). Funcionan con las IR de fábrica, con las de usuario y con NAM + IR. Con los dos en Off suena igual que la v2.
- Todo lo de la v2 se mantiene: NAM + IR, 37 amplis y 17 delays.
- Al flashear, revisa los huecos NAM y vuelve a subir las capturas que falten.

### AMPCUBE Custom Studio 3.0 (Windows y Android)

- **Asistente de tono:** describes el sonido (un grupo, una canción, un guitarrista o un estilo, con matices como «más ganancia», «oscuro», «drop C») y crea un preset solo con los modelos del AMPCUBE, sin NAM ni IR de usuario.
  - Se carga en el equipo **sin guardar** y pasas al editor para retocarlo; «Guardar en…» lo guarda en la posición que elijas y «Descartar» vuelve al preset anterior.
  - La base del asistente reconoce más de 100 grupos, guitarristas y canciones y unos 30 estilos, sin Internet.
  - **IA integrada opcional:** en Android o en Windows se descarga una vez un modelo Qwen 2.5 (Apache 2.0) y funciona sin Internet ni cuentas. En Windows usa la tarjeta gráfica si puede. Con «✦ Crear versión B con la IA» comparas las dos propuestas en el equipo, con el volumen igualado y un ajuste fino de volumen.
  - Los limpios no rompen (ganancia y master contenidos) y los cortes del IR son suaves.
- **Métricas NAM vs CLONE** al convertir una captura: modelo (A1/A2, arquitectura, parámetros), fidelidad, error y relación señal/error por intensidad, diferencia de volumen y respuesta en frecuencia superpuesta, con diferencias por bandas.
- **13 huecos NAM** con el firmware v4 (se detecta solo).
- **Low Cut y High Cut:** botón para activarlos o desactivarlos y comparar.
- **Android pensado para el móvil:** deslizadores grandes en lugar de perillas, barra fija de bloques encima del inspector, deslizar el nombre para cambiar de preset, «IR y NAM» con pestañas.
- **Más fluido:** al cargar un preset del asistente solo se envía lo que cambia; con la app en segundo plano no se consulta el equipo.
- **TONE3000 integrado:** nueva pestaña con la web de TONE3000 dentro del editor, con atrás, inicio y recargar. Al descargar una captura, el editor la recoge (no va a la carpeta de descargas), la convierte en cuanto llega y la carga en el hueco NAM que elijas. Admite `.nam`, `.zip` con varias capturas e IR `.wav` para los huecos de User IR. La conexión con el AMPCUBE no se corta.
- **Low Cut y High Cut** en el bloque IR, mostrados y editados en Hz («90 Hz», «6,5k», «Off»).
- **Conversión NAM → Clone mejorada:**
  - tiene en cuenta el filtro de continua del equipo y amplía el rango de ganancia del saturador;
  - ajusta el volumen real de salida: antes, algunas capturas A2 pequeñas salían unas 100 veces más altas;
  - el refinado final usa Adam y después L-BFGS.

  | Captura | Antes | Ahora |
  |---|---|---|
  | A2 estándar | 82 % | 85 % |
  | A1 estándar | 53 % | 66 % |
  | Friedman con TS | 18 % | 65 % |
  | Peavey 6505 | 29 % | 74 % |

- **Windows:** el editor usa Microsoft Edge WebView2 (incluido en Windows 11 y con Edge en Windows 10) en lugar de una ventana de Edge en modo app.
- **Android:** el editor, la pestaña TONE3000 y la conversión se ven bien en el móvil, sin scroll lateral, aunque el sistema tenga la letra grande.
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
