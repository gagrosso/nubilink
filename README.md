# Nubilink

Sitio web institucional de **Nubilink** — *AWS Select Consulting Partner* (AR · ES · US).
Diseño, migración y operación de infraestructura en AWS.

🌐 **Sitio en vivo:** https://gagrosso.github.io/nubilink/

## Sobre el proyecto

Página web de una sola página (single-file) totalmente autosuficiente: **HTML + CSS + JavaScript vanilla**, sin frameworks ni dependencias externas (solo la fuente Poppins de Google Fonts). Todo el sitio vive en [`index.html`](index.html).

### Funcionalidades

- **4 secciones**: Inicio, Nubilink (empresa), Servicios y Contacto, con navegación tipo SPA.
- **Bilingüe** español / inglés con un selector que actualiza también `<html lang>` y el título.
- **Formulario de contacto** con validación y estado de éxito.
- **Responsive** desde 375px, con menú hamburguesa en móvil.
- Respeta `prefers-reduced-motion`.

## Desarrollo local

No requiere build. Cualquier servidor estático sirve:

```bash
python3 -m http.server 4321
# abrir http://localhost:4321
```

## Despliegue

Publicado con **GitHub Pages** desde la rama `main` (raíz del repo). Cada push a `main` actualiza el sitio automáticamente.

---

Implementado a partir de un diseño de [Claude Design](https://claude.ai/design).
