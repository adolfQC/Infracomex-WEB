# Infracomex — sitio web

Sitio de una sola página para Infracomex (expansión comercial, asesoría empresarial e inversión inmobiliaria).
Portada con historia 3D en scroll (three.js r128 desde CDN) y texturas de la Tierra de NASA Blue Marble / Black Marble (dominio público).

## Estructura
- `index.html` — toda la página (HTML, CSS y JS en un solo archivo)
- `assets/` — texturas de la Tierra usadas por la portada 3D

## Ver en local
Las texturas no cargan abriendo el archivo con doble clic (bloqueo CORS de `file://`). Sirve la carpeta:

    python3 -m http.server 8000
    # abrir http://localhost:8000

## Publicar gratis
GitHub Pages: Settings → Pages → Source: "Deploy from a branch" → rama `main`, carpeta `/ (root)`.

## Pendientes por confirmar con Carlos
- Nombres de empresas asesoradas (hoy son espacios "por confirmar")
- Logo oficial, fotos de proyectos y número de WhatsApp
- Un brief real de cadena para calibrar el simulador de scoring
- Prueba de rendimiento en celulares de gama media

## Nota
Las funciones de IA dentro de la página (lectura de mensajes de propietarios, redacción de fichas) usan la capacidad de Claude del artifact y quedan desactivadas fuera de claude.ai; la página tiene respaldo heurístico y sigue funcionando sin ellas.
