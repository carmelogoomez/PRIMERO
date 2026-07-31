# PizzPlass — Blog & web informativa 🍕

Sitio web informativo tipo blog para **PizzPlass**, empresa de **pizza napolitana para eventos** (bodas, comuniones, cumpleaños, eventos de empresa…), fundada por los hermanos **Leo y Juan Antonio**, pizzaiolos napolitanos.

## ¿Qué incluye?

Sitio **estático** (HTML + CSS + JavaScript, sin dependencias ni build). Se abre directamente en el navegador.

### Páginas

| Página | Archivo | Contenido |
|---|---|---|
| Inicio | `index.html` | Hero, propuesta de valor, hermanos, eventos, blog destacado, CTA |
| Nosotros | `nosotros.html` | Historia de Leo y Juan Antonio, línea de tiempo y valores |
| Eventos | `eventos.html` | Servicios (bodas, comuniones, cumpleaños, empresa), proceso y carta |
| Blog | `blog.html` | Listado de artículos |
| Contacto | `contacto.html` | Formulario de presupuesto e información de contacto |

### Artículos del blog (`/blog/`)

- `pizza-napolitana-autentica.html` — Qué hace auténtica a una pizza napolitana
- `pizza-en-tu-boda.html` — Pizza napolitana en tu boda
- `historia-pizzplass.html` — Dos hermanos, un horno y mucha ilusión
- `secretos-masa-48-horas.html` — La fermentación de 48 horas
- `como-elegir-catering-evento.html` — Cómo elegir el catering perfecto
- `horno-lena-espectaculo.html` — El horno de gas portátil como experiencia

## Estructura

```
.
├── index.html
├── nosotros.html
├── eventos.html
├── blog.html
├── contacto.html
├── blog/                  # artículos individuales
├── css/styles.css         # sistema de diseño
├── js/main.js             # menú móvil, animaciones, formulario (email + WhatsApp)
└── assets/logo.jpg        # logo de la marca
```

## Cómo verlo

Abre `index.html` en el navegador, o sirve la carpeta con un servidor local:

```bash
python3 -m http.server 8000
# luego visita http://localhost:8000
```

## Notas

- **Diseño:** paleta italiana (tomate, albahaca, dorado y crema), tipografía serif para titulares y responsive completo (móvil incluido).
- **Datos de contacto:** Instagram [@pizzplass_pizzas](https://www.instagram.com/pizzplass_pizzas), TikTok `pizzplass.pizzas`, WhatsApp `675 26 49 67` y email `pizzplasspizzas@gmail.com` son reales.
- **Logo:** `assets/logo.jpg` (logo real de la marca).
- **Formulario de contacto:** funcional sin backend. Envía por **email vía [FormSubmit](https://formsubmit.co)** (requiere activar el correo una vez) y ofrece un botón de **WhatsApp** con los datos prerrellenados. Todos los campos son obligatorios.
- **SEO:** cada página incluye `title`, `meta description`, `canonical`, Open Graph y Twitter Card. Datos estructurados JSON-LD: `FoodEstablishment` + `WebSite` (inicio), `BlogPosting` (artículos), `BreadcrumbList` y `ContactPage`. `sitemap.xml` y `robots.txt` incluidos.
- **Publicación:** GitHub Pages sirviendo `master` (raíz) con dominio propio `pizzplass.es` (archivo `CNAME`).
