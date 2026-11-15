# NEXUS

Herramientas útiles con diseño Liquid Glass (cristal, blur, tema claro/oscuro). Flutter + SQLite, sin IA. Windows y Android.

**Herramientas:** dispositivo · notas · test de velocidad · benchmark · QR · enlaces (solo metadatos, sin descargas) · MP3/MP4 · conversor · compresor de imágenes · PDF · contraseñas · analizador de red.

## Compilar (automático)
1. Sube el proyecto a GitHub (rama `main`).
2. Pestaña **Actions → Build NEXUS** (se lanza solo con cada push, o con *Run workflow*).
3. Al terminar, descarga en *Artifacts*: `nexus-android-apk` (APK) y `nexus-windows` (ZIP con el .exe).

## Compilar en local
```
bash tool/bootstrap.sh   # genera android/ y windows/
flutter pub get
flutter run -d windows   # o android
```

## Añadir una herramienta
Crea `lib/tools/mi_tool.dart` (un widget con `GlassPage`) y regístrala en `lib/tools/registry.dart`.

## Estado
Código **no compilado todavía** (el entorno de desarrollo no tenía Flutter). Ver `NEXUS_PROGRESS.md`.
