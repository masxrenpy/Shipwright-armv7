# Ship of Harkinian – Android 32-bit (armv7) beta · FAQ

Unofficial community build. **No game files are included: you need your own legally obtained ROM.**

---

## ES · Preguntas frecuentes

**¿Cómo la instalo?**
1. Si tienes otro Ship of Harkinian instalado (por ejemplo el port original), desinstálalo primero: están firmados con claves distintas. Haz antes una copia de la carpeta `SOH`.
2. Instala el APK de la última release (permite "instalar apps de fuentes desconocidas").
3. Copia tu ROM a `/storage/emulated/0/SOH/` y comprueba que el nombre termine en `.z64` (o `.n64` / `.v64`).
4. Abre la app y responde **Sí** a "generar archivos" y **Sí** a "procesar las ROMs encontradas".

**La extracción tarda mucho. ¿Está colgada?**
En teléfonos lentos puede tardar de 15 a 30 minutos. La barra dice "Starting Up" al principio y solo empieza a avanzar cuando termina el primer bloque de archivos. Deja la app abierta, la pantalla encendida y el cargador conectado. Si llevas más de una hora sin avance, abre un Issue con los archivos de `SOH/logs/`.

**No detecta mi ROM.**
Comprueba que está directamente en `/storage/emulated/0/SOH/` (no en una subcarpeta), que la extensión es `.z64`, `.n64` o `.v64`, y que la ROM es una versión compatible. Si no la detecta, la app abre el selector de archivos; usa la app de archivos del sistema ("Archivos" / "Documentos").

**Actualicé la app. ¿Tengo que extraer otra vez?**
Normalmente no: desde la beta 2 la app conserva `oot.o2r` al actualizar. Solo se pedirá extraer de nuevo si una versión lo indica en sus notas.

**Los caminos de tierra desaparecen.**
En esta build el ajuste *Enhancements → Fixes → Graphical Fixes → Fix Vanishing Paths* viene en **No Vanish** por defecto. Puedes cambiarlo en el menú.

**Con 30 o 60 FPS el audio se corta.**
Los FPS por encima de 20 se consiguen interpolando fotogramas, y esto cuesta CPU. En teléfonos lentos lo más estable es dejar 20 FPS. Cuéntanos tu modelo en un Issue si te pasa en uno más potente.

**Partes de los modelos no se ven (GPU PowerVR).**
Está arreglado en esta build. Si usas otra GPU y ves algo parecido, crea una carpeta vacía llamada `gfx_nowrap` dentro de `SOH`, reinicia la app y cuéntanos si cambia algo (borra la carpeta para volver al comportamiento normal). La carpeta `gfx_wrap` hace lo contrario.

**¿Cómo uso mods?**
Copia los archivos `.o2r` / `.otr` del mod a la carpeta `SOH` (la app también crea `SOH/mods`; sigue las instrucciones del README original) y actívalos en *Enhancements → Mods*. Muchos mods antiguos no son compatibles con versiones recientes.

**La app se cierra o falla. ¿Qué adjunto al reportarlo?**
Abre un Issue y adjunta, si existen, estos archivos de `SOH/logs/`:
`device-info.txt`, `exit-reasons.txt`, `java-crash.txt`, `native-crash.txt`, `gfx-diag.txt`, `extract-diag.txt`, `java-diag.txt`, `zapd.txt` y el `.log` más reciente.

---

## EN · FAQ

**How do I install it?**
1. If another Ship of Harkinian is installed (e.g. the original port), uninstall it first: they are signed with different keys. Back up your `SOH` folder first.
2. Install the APK from the latest release (allow "install unknown apps").
3. Copy your ROM to `/storage/emulated/0/SOH/` and make sure the name ends in `.z64` (or `.n64` / `.v64`).
4. Open the app and answer **Yes** to "generate files" and **Yes** to "process the ROMs found".

**Extraction takes very long. Is it stuck?**
On slow phones it can take 15 to 30 minutes. The bar says "Starting Up" at first and only moves once the first group of files is done. Keep the app open, the screen on and the charger connected. If there is no progress after an hour, open an Issue with the files from `SOH/logs/`.

**My ROM is not detected.**
Check that it is directly in `/storage/emulated/0/SOH/` (not in a subfolder), that the extension is `.z64`, `.n64` or `.v64`, and that the ROM is a supported version. If it is not detected the app opens the file picker; use the system file app ("Files" / "Documents").

**I updated the app. Do I have to extract again?**
Normally no: since beta 2 the app keeps `oot.o2r` when updating. You will only be asked to extract again if a release says so in its notes.

**Dirt paths vanish.**
In this build *Enhancements → Fixes → Graphical Fixes → Fix Vanishing Paths* defaults to **No Vanish**. You can change it in the menu.

**Audio stutters at 30 or 60 FPS.**
Anything above 20 FPS is achieved by interpolating frames, which costs CPU. On slow phones 20 FPS is the most stable setting. If it happens on a faster phone, open an Issue with your model.

**Parts of models are not drawn (PowerVR GPUs).**
Fixed in this build. If you have another GPU and see something similar, create an empty folder named `gfx_nowrap` inside `SOH`, restart the app and tell us whether anything changes (delete the folder to go back to normal). The `gfx_wrap` folder does the opposite.

**How do I use mods?**
Copy the mod's `.o2r` / `.otr` files to the `SOH` folder (the app also creates `SOH/mods`; follow the original README) and enable them in *Enhancements → Mods*. Many old mods are not compatible with recent versions.

**The app closes or fails. What do I attach?**
Open an Issue and attach, if they exist, these files from `SOH/logs/`:
`device-info.txt`, `exit-reasons.txt`, `java-crash.txt`, `native-crash.txt`, `gfx-diag.txt`, `extract-diag.txt`, `java-diag.txt`, `zapd.txt` and the most recent `.log`.
