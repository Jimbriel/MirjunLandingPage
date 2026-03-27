# MIRJUN S.A. — Landing Page Corporativa

> **"Tu proyecto, nuestro compromiso."**  
> Sitio web corporativo para MIRJUN S.A. — Guayaquil, Ecuador.

![Estado](https://img.shields.io/badge/estado-producción-6A2B86?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

## 📋 Descripción

Landing page estática de tres páginas para **MIRJUN S.A.**, empresa especializada en:

- 🏗️ **Construcción e Infraestructura** — viviendas, remodelaciones, adecuaciones.
- ❄️ **Climatización y Refrigeración** — instalación y mantenimiento de sistemas HVAC.
- 🔧 **Ingeniería Técnica** — mantenimiento industrial, redes hidrosanitarias, ascensores.

El diseño sigue el sistema **"Architectural Monolith"**: tipografía editorial, paleta monocromática con acento en morado `#6A2B86`, y composición asimétrica de alto impacto visual.

---

## 🗂️ Estructura del Proyecto

```
/
├── index.html          ← Página de inicio
├── empresa.html        ← Página institucional
├── contact.html        ← Página de contacto
│
├── assets/
│   ├── css/
│   │   └── styles.css  ← Estilos globales y utilitarios
│   ├── js/
│   │   └── main.js     ← Lógica de UI: menú, animaciones, footer
│   └── img/            ← Fotografías del portafolio
│
├── doc/
│   └── CATALOGO MIRJUN SA 2024.pdf
│
├── DESIGN.md           ← Sistema de diseño (tokens, tipografía, componentes)
├── info.md             ← Copy de referencia del sitio
├── README.md           ← Este archivo
└── README.txt          ← Versión de texto plano
```

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| **HTML5 semántico** | Estructura de las páginas |
| **Tailwind CSS** (CDN) | Sistema de utilidades CSS |
| **CSS personalizado** | Gradientes, animaciones, tokens de marca |
| **JavaScript vanilla** | Menú móvil, animaciones `reveal`, año en footer |
| **Google Fonts** | Manrope (headlines) + Inter (body) |
| **Google Material Symbols** | Iconografía |
| **Google Maps Embed** | Mapa en página de contacto |

---

## 📄 Páginas

### `index.html` — Inicio
- Hero a pantalla completa con fotografía y CTA
- Sección "Quiénes somos" con estadísticas clave
- Tarjetas de servicios principales
- Galería de proyectos destacados (IESS Los Ceibos, CNT Guayas)
- CTA final hacia WhatsApp

### `empresa.html` — Nuestra Empresa
- Header editorial tipográfico
- Historia de la empresa (fundada 2022, Guayaquil)
- Misión y Visión en doble columna
- Valores corporativos con tarjetas interactivas
- Trayectoria cronológica: 2022 → 2023 → 2024

### `contact.html` — Contacto
- Formulario de consulta especializada (tipo de servicio, descripción)
- Panel de información directa (email, teléfono, dirección)
- Mapa embebido de Google Maps

---

## 🎨 Sistema de Diseño

Ver [`DESIGN.md`](./DESIGN.md) para el detalle completo.

| Token | Valor | Uso |
|---|---|---|
| `primary` | `#6A2B86` | Acciones, highlights, CTA |
| `surface` | `#fbf9f8` | Fondo principal |
| `on-surface` | `#1b1c1c` | Texto principal |
| `Manrope` | 800 weight | Headlines y display text |
| `Inter` | 400/500/600 | Cuerpo de texto y labels |

---

## 🚀 Uso Local

Este proyecto es **completamente estático**. No requiere servidor ni dependencias de Node.js.

1. Clona o descarga el repositorio.
2. Abre `index.html` directamente en tu navegador.
3. Navega entre las páginas usando el menú de navegación.

```bash
git clone https://github.com/Jimbriel/MirjunLandingPage.git
cd MirjunLandingPage
# Abrir index.html en el navegador
```

> 💡 Para una mejor experiencia de desarrollo, usa la extensión **Live Server** en VS Code.

---

## 📞 Contacto de la Empresa

| Canal | Detalle |
|---|---|
| 📧 Email | servicios@mirjun.com |
| 📱 Teléfono | 098 674 6837 |
| 💬 WhatsApp | [wa.me/593979448281](https://wa.me/593979448281) |
| 📍 Ciudad | Guayaquil, Ecuador |

---

## 📁 Repositorio

**GitHub:** [github.com/Jimbriel/MirjunLandingPage](https://github.com/Jimbriel/MirjunLandingPage)

---

*© 2025 MIRJUN S.A. — Architectural Integrity.*
