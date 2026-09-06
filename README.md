# Gedetca Soft — Descargas

Página pública de descarga del software de Gedetca:

- **Escritorio (Windows):** `GedetcaWebEscritorio_Setup.exe`
- **Android (teléfonos y handheld):** `Gedetca_soft.apk`

Los instaladores se publican como *Releases* de este repo. La página
(`index.html`, servida por GitHub Pages) siempre apunta a la última:

    https://kalimusic0.github.io/gedetca-descargas/

## Publicar una versión nueva

```bash
gh release create v1.0.1 \
  "C:/gedetca-apk/GedetcaWebEscritorio_Setup.exe" \
  "C:/gedetca-apk/app-debug.apk#Gedetca_soft.apk" \
  --title "v1.0.1" --notes "Cambios..."
```

O reemplazar los assets de la release actual:

```bash
gh release upload v1.0 "C:/gedetca-apk/app-debug.apk#Gedetca_soft.apk" --clobber
```
