# MEMORIA DEL PROYECTO — DECOAS Santa Bárbara

**Última actualización:** 4 de junio de 2026
**Cliente:** José David Mejia
**Proyecto:** Revista digital DECOAS Santa Bárbara
**Ubicación:** `C:\xampp\htdocs\revista\`

---

## 📌 ESTADO GENERAL

| Componente | Estado |
|---|---|
| Página principal (`index.html`) | ✅ **Completa** — con contenido del DOCX |
| Archivos de la plantilla original | ✅ **Eliminados** — solo conservamos `index.html` |
| CSS — Paleta de colores | ✅ Verde temático aplicado |
| CSS — Footer | ✅ Colores corregidos para legibilidad |
| CSS — Diseño original | ✅ **Preservado** (sin modificar estructura, clases, efectos) |

---

## 📄 ARCHIVOS DEL PROYECTO

### HTML
- **`index.html`** — Página principal con contenido DECOAS del DOCX
- **`recursos.html`** — Página de Recursos Educativos con galería de videos desde Google Drive

### JavaScript
- **`videos-data.js`** — Archivo de datos con IDs de videos de Google Drive (editar aquí para actualizar la videoteca)

### CSS
| Archivo | Descripción |
|---|---|
| `style.css` | Estilos base del template — **sin modificar** |
| `css/bootstrap.css` | Framework Bootstrap — **sin modificar** |
| `css/font-awesome.min.css` | Iconos FontAwesome — **sin modificar** |
| `css/responsive.css` | Estilos responsive — **sin modificar** |
| `css/colors.css` | Colores principales → **cambiado a verde** `#2e7d32` (original: azul `#3197d6`) |
| `css/version/tech.css` | Estilos de versión tech → **adaptado a DECOAS** con paleta verde |

### Imágenes
| Archivo | Uso |
|---|---|
| `images/logo_decoas.jpeg` | Logo en navbar y footer |
| `images/logo_decoas_256.jpeg` | Favicon del sitio |
| `images/decoasSB.jpeg` | Hero principal y secciones |
| `images/decoasSB_1.jpeg` | Misión/Visión, Beneficios, etc. |
| `images/calendario_decoas.jpeg` | Banner calendario y sección CODEAS |

---

## 🎨 PALETA DE COLORES DECOAS

| Color | Código | Uso |
|---|---|---|
| Verde oscuro | `#1b5e20` | Navbar, hover de enlaces, títulos footer |
| Verde medio | `#2e7d32` | Color principal, botones, enlaces, texto footer |
| Verde medio claro | `#388e3c` | Enlaces en footer |
| Verde claro | `#4caf50` | Gradiente de botones |
| Naranja | (bg-orange) | Tags/categorías (original del template) |

### Navbar
- Fondo: Gradiente `#1b5e20 → #388e3c`
- Texto: Blanco `#ffffff`
- Sombras: `0 0 10px rgba(0,0,0,0.4)`

### Footer
- Fondo: `#edeff2` con patrón `footer.png`
- Texto `p`: `#2e7d32` (corregido — antes era `#c8e6c9`, ilegible)
- Enlaces `a`: `#388e3c` (corregido)
- Títulos: `#1b5e20` (corregido)
- Hover enlaces: `#1b5e20`
- Borde widgets: `rgba(0,0,0,0.08)`

---

## 📋 PÁGINA DE RECURSOS (`recursos.html`)

### Navbar
- Mismo navbar que index.html con enlace activo a "Recursos"
- Enlace a Recursos agregado también en el navbar de `index.html`

### Page Title
- Título: "Recursos Educativos" con icono de YouTube
- Breadcrumb: Inicio > Recursos

### Contenido principal
- **Descripción** del programa DECOAS en la videoteca
- **Galería dinámica de videos** — Grid de 2 columnas que se carga desde `videos-data.js`
  - Cada video se muestra en una tarjeta con:
    - Reproductor de Google Drive embebido (iframe responsivo 16:9)
    - Título del video (enlace para abrir en Google Drive)
    - Descripción breve
  - Contador automático de videos
- Banner del calendario DECOAS

### Sidebar y Footer
- Idénticos a `index.html` (logo, proyectos, beneficios, redes sociales, calendario)

### Cómo actualizar los videos
1. Abrir `videos-data.js`
2. Modificar/agregar/quitar objetos en el array `videosData`
3. Cada video requiere: `id`, `title`, `description`
4. El ID se obtiene del enlace de Google Drive: `/d/ID_DEL_VIDEO/view`
5. **Los videos deben estar compartidos como "Cualquier persona con el enlace"**

---

## 📋 ESTRUCTURA DEL INDEX.HTML

### Navbar
- Logo con `logo_decoas.jpeg`
- Enlaces: Inicio, ¿Qué es DECOAS?, Misión y Visión, Beneficios, Noticias, Proyectos, Contacto

### Hero (Masonry)
- 3 slots con imágenes y overlay shadoweffect (mismo diseño original)
- `decoasSB.jpeg` (slot grande 50%), `decoasSB_1.jpeg` (25%), `calendario_decoas.jpeg` (25%)

### Contenido principal
Secciones del DOCX incluidas:
1. **Bienvenida** — Texto de introducción completo
2. **Misión y Visión** — Con imagen y texto completo
3. **¿Qué es DECOAS?** — Historia del departamento
4. **Banner calendario** — Imagen `calendario_decoas.jpeg`
5. **Beneficios** — Para escuelas y comunidades (punto por punto)
6. **Concientización Ambiental** — Mensaje con blockquote
7. **Noticias y Actividades** — Resumen
8. **Proyectos Ambientales** — Plantatón, huertos, reciclaje
9. **CODEAS** — Comités de educación ambiental
10. **Recursos Educativos** — Guías y manuales
11. **Reconocimientos** — Escuelas destacadas y aliados

### Sidebar (3 columnas)
- Logo DECOAS
- Widget "Sobre DECOAS"
- Widget "Proyectos" (Plantatón, Huertos, Reciclaje)
- Widget "Beneficios Clave" (con estrellas)
- Widget "Síguenos" (Facebook, Twitter, Instagram, YouTube)
- Banner calendario

### Footer
- Logo + nombre + eslogan
- Redes sociales
- **Copyright:** `© 2025 DECOAS Santa Bárbara. Unidad de Tecnología Informática — DDE Santa Bárbara.`

---

## ⚠️ PENDIENTE PARA PRÓXIMA SESIÓN

- [ ] **Crear páginas secundarias** (artículos, categorías, contacto, etc.)
- [ ] Enlazar redes sociales reales (Facebook, Twitter, Instagram, YouTube)
- [ ] Agregar contenido específico como galería de fotos, eventos del calendario, etc.
- [ ] Verificar que todas las imágenes se carguen correctamente
- [ ] Probar responsive en diferentes dispositivos

---

## 🔧 NOTAS TÉCNICAS

- La plantilla original usa **Bootstrap 4** (clases `navbar-toggleable-md`, `mr-auto`, etc.)
- Tipografía: **Poppins** (Google Fonts)
- Los efectos hover/shadow del template original se mantienen intactos
- Smooth scroll implementado via enlaces `#` a secciones
- Los archivos de la plantilla original fueron eliminados (el cliente tiene copia de respaldo)
