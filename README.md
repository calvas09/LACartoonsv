# LACartoons TV

App para Android TV / Fire TV que abre https://www.lacartoons.com/ dentro de un WebView, sin modificar la página.

## Obtener el APK sin instalar nada (GitHub Actions)
1. Crea un repositorio en GitHub y sube TODO el contenido de esta carpeta (incluida `.github`).
2. Entra a la pestaña **Actions** > **Build LACartoons TV APK** > **Run workflow**.
3. Al terminar, descarga el artefacto **LACartoonsTV-APK** (contiene `app-debug.apk`).

## Con Android Studio
Abre esta carpeta, deja que sincronice y usa **Build > Build APK(s)**.
Salida: `app/build/outputs/apk/debug/app-debug.apk`

## Instalar en la TV
- Fire TV: activa Opciones de desarrollador y Depuración ADB, luego `adb connect IP_DE_LA_TV` y `adb install app-debug.apk`.
- O sube el APK a un enlace/nube y descárgalo con la app Downloader.
