# Ship of Harkinian – Android 32-bit (armv7) – BETA

> **Unofficial community build. Beta software.** Based on the Android port of Ship of Harkinian
> (please-be-nice/Shipwright-android). Not affiliated with Nintendo or the Ship of Harkinian team.
> **No game files are included. You must provide your own legally obtained ROM.**

## ES – Resumen
Compilación para Android de **32 bits (armeabi-v7a)**, pensada para teléfonos con sistema de 32 bits
(por ejemplo Redmi 9A, Helio G25). Esta es una **beta**: puede fallar y necesitamos testers.

### Qué incluye
- Build `armeabi-v7a` (también instala en teléfonos de 64 bits, pero allí el port original rinde mejor).
- Arreglo del mezclador de audio NEON para ARM de 32 bits.
- Detección automática de la ROM en la carpeta `SOH` (evita el selector de archivos, que falla en algunos teléfonos).
- Selector de archivos más robusto (muestra un aviso en vez de quedarse colgado).
- Arreglo de render en GPU **PowerVR**: partes de modelos que no se dibujaban (caballo, castillo).
- Registros extra en `SOH/logs/` para diagnosticar problemas.

### Instalación
1. Si tienes instalado otro Ship of Harkinian (por ejemplo el port original), **desinstálalo primero**
   (están firmados con claves distintas). Haz antes una copia de la carpeta `SOH`.
2. Instala el APK (permite "instalar apps de fuentes desconocidas").
3. Copia tu ROM a `/storage/emulated/0/SOH/` y asegúrate de que termine en `.z64` (o `.n64` / `.v64`).
4. Abre la app: responde **Sí** a "generar archivos" y **Sí** a "procesar las ROMs encontradas".
   La extracción puede tardar bastante en teléfonos lentos; mantén la pantalla encendida y el cargador conectado.

### Problemas conocidos
- El rendimiento en teléfonos de gama baja es limitado (20 FPS por defecto).
- Con 30/60 FPS el audio puede cortarse en CPUs lentas.
- Mantén el MSAA en 1.
- Los mods no han sido probados en esta build.

### Cómo reportar un error
Abre un *Issue* e incluye: modelo del teléfono, versión de Android, GPU y estos archivos de `SOH/logs/` si existen:
`*.log`, `gfx-diag.txt`, `extract-diag.txt`, `java-diag.txt`, `zapd.txt`.

Opciones para testers (crear una carpeta vacía dentro de `SOH/`):
`gfx_nowrap` fuerza el arreglo de render en cualquier GPU; `gfx_wrap` lo desactiva.

---

## EN – Summary
Android **32-bit (armeabi-v7a)** build for phones running a 32-bit-only system (e.g. Redmi 9A / Helio G25).
This is a **beta** and we need testers.

### What's included
- `armeabi-v7a` build (it also installs on 64-bit phones, but the original port is better there).
- NEON audio mixer fix for 32-bit ARM.
- Automatic ROM detection in the `SOH` folder (avoids the file picker, which fails on some phones).
- More robust file picker (shows a message instead of hanging).
- Rendering fix for **PowerVR** GPUs: model parts that were not drawn (horse, castle).
- Extra logs in `SOH/logs/` for troubleshooting.

### Install
1. If another Ship of Harkinian is installed (e.g. the original port), **uninstall it first** (different signing keys).
   Back up your `SOH` folder first.
2. Install the APK (allow "install unknown apps").
3. Copy your ROM to `/storage/emulated/0/SOH/` and make sure it ends in `.z64` (or `.n64` / `.v64`).
4. Open the app: answer **Yes** to "generate files" and **Yes** to "process the ROMs found".
   Extraction can take a long time on slow phones; keep the screen on and the charger connected.

### Known issues
- Performance on low-end phones is limited (20 FPS by default).
- At 30/60 FPS audio may stutter on slow CPUs.
- Keep MSAA at 1.
- Mods have not been tested on this build.

### Reporting bugs
Open an *Issue* with: phone model, Android version, GPU, and these files from `SOH/logs/` if present:
`*.log`, `gfx-diag.txt`, `extract-diag.txt`, `java-diag.txt`, `zapd.txt`.

Tester options (create an empty folder inside `SOH/`):
`gfx_nowrap` forces the rendering fix on any GPU; `gfx_wrap` disables it.
