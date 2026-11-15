# NEXUS_PROGRESS

## Fase 1 (hecha: código escrito)
- Núcleo: tema Liquid Glass (`core/glass.dart`), SQLite (`core/db.dart`), guardado de archivos (`core/files.dart`).
- 12 herramientas en `lib/tools/`, registradas en `registry.dart`.
- CI: `.github/workflows/build.yml` + `tool/bootstrap.sh` (genera android/windows y parchea permisos).

## NO verificado
- Nada se ha compilado ni ejecutado aún. Es probable que el primer build de CI muestre errores menores de API/versiones: corregirlos es el siguiente paso.

## Limitaciones conocidas
- Multimedia MP3/MP4: solo Windows y requiere FFmpeg en PATH. Android pendiente (integrar librería FFmpeg).
- PDF: solo imágenes→PDF y texto→PDF. Pendiente: unir/dividir.
- Lector QR con cámara: solo Android. Windows pendiente (leer desde imagen).
- Enlaces: solo análisis + metadatos oEmbed (YouTube/TikTok). Sin descargas, por términos de las plataformas.
- Hay que cambiar la firma de release del APK (usa firma debug por defecto).

## Siguientes pasos
1. Push a GitHub → revisar logs de Actions → arreglar errores.
2. Probar en Windows y Android reales.
3. Pendientes de arriba.
