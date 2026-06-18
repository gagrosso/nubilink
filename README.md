# Nubilink

Sitio web institucional de **Nubilink** — *AWS Select Consulting Partner* (AR · ES · US).
Diseño, migración y operación de infraestructura en AWS.

🌐 **Sitio en vivo:** https://gagrosso.github.io/nubilink/

## Sobre el proyecto

Página web de una sola página (single-file) totalmente autosuficiente: **HTML + CSS + JavaScript vanilla**, sin frameworks ni dependencias externas (solo la fuente Poppins de Google Fonts). Todo el sitio vive en [`index.html`](index.html).

### Funcionalidades

- **4 secciones**: Inicio, Nubilink (empresa), Servicios y Contacto, con navegación tipo SPA.
- **Bilingüe** español / inglés con un selector que actualiza también `<html lang>` y el título.
- **Capa de movimiento "Líneas de Luz"**: hero con aurora WebGL, revelados al scroll, acto de servicios con travelling horizontal, count-up del 25%, CTA magnético y scroll suave (GSAP + Lenis vía CDN). Degrada a un sitio estático si un CDN falla o si el usuario pidió menos movimiento.
- **Formulario de contacto** con validación, accesibilidad (aria-live) y entrega real.
- **Responsive** desde 375px, con menú hamburguesa en móvil.
- Respeta `prefers-reduced-motion` y `pointer: coarse`.

### Formulario de contacto

Por defecto el formulario abre el correo del visitante con un borrador a `info@nubilink.com` (más botones directos de e-mail y WhatsApp). Para envío silencioso en segundo plano, crea una clave gratuita en [web3forms.com](https://web3forms.com) (1 minuto, sin backend) y pégala en la constante `FORM_ACCESS_KEY` dentro de `index.html`.

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
