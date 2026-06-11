# PFO2 — Landing Page Agentic

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat&logo=githubpages&logoColor=white)

**Dos agentes de IA. Un mismo prompt. Dos implementaciones de una Landing Page.**

Proyecto correspondiente a la Prueba de Formación Obligatoria N° 2 (Individual) de la materia **Desarrollo de Sistemas Web (Front End)**.

---

## Datos del Estudiante

| | |
|---|---|
| **Nombre** | Marcelo Javier Moreno |
| **Carrera** | Tecnicatura en Desarrollo de Software |
| **Institución** | IFTS N° 29 |
| **Materia** | Desarrollo de Sistemas Web (Front End) |
| **Curso** | 2° D |
| **Instancia** | PFO 2 — Individual |

---

## Deploy Unificado

> **GitHub Pages:** [https://javiacode.github.io/pfo2-landing-page-agentic/](https://javiacode.github.io/pfo2-landing-page-agentic/)

Una vez deployado, este único enlace dirige a la **portada** (`index.html`) desde la cual se accede a las tres secciones del proyecto:
1. Prompt original utilizado
2. Landing Page — Agente 1 (sdd-orchestrator / deepseek-v4-pro)
3. Landing Page — Agente 2 (Gemini / 3.5 Flash)

---

## Estructura del Proyecto

```
/
├── index.html              ← Portada unificada con 3 accesos directos
├── prompt.html             ← Texto plano del prompt original
├── README.md               ← Este archivo
├── Opencode/
│   └── index.html          ← Landing Page generada por Agente 1
└── Antigravity/
    ├── index.html          ← Landing Page generada por Agente 2
    ├── hero_bg.png
    └── about_gym.png
```

---

## Prompt Original

El siguiente prompt fue estructurado y refinado iterativamente en [Gemini](https://gemini.google.com/share/eefb842d33f5) antes de ser entregado a ambos agentes:

> **[CONTEXTO Y ROL]**
> Actúas como un Ingeniero de Software Senior y Diseñador UX/UI experto. Tu objetivo es generar de forma 100% autónoma todos los archivos necesarios (HTML, CSS y JavaScript si aplica) para una Landing Page profesional, visualmente atractiva, responsiva y totalmente limpia.
>
> **[TEMÁTICA]**
> El sitio web estará dedicado a: un gimnasio de streetlifting llamado "El Templo".
>
> **[REQUISITOS ESTRUCTURALES DE LA INTERFAZ]**
> Debes incluir e implementar obligatoriamente las siguientes secciones en un diseño de página única (Single Page Application estética):
> 1. Cabecera (Header): Menú de navegación moderno, logo (marcador de posición) y enlaces internos responsivos.
> 2. Hero Section: Título principal impactante (Headline), subtítulo persuasivo y un botón destacado de llamada a la acción (CTA).
> 3. Sobre Nosotros: Breve descripción narrativa de la marca/servicio con un diseño limpio.
> 4. Servicios o Características: Grilla o contenedor con las características principales o planes del servicio, usando iconos o componentes visuales atractivos.
> 5. Testimonios: Sección de reseñas o prueba social con avatares y citas de clientes de ejemplo.
> 6. Formulario de Contacto: Maquetado visual completo de un formulario (campos de Nombre, Email, Mensaje y botón de envío). No requiere funcionalidad backend, pero debe ser interactivo en el frontend.
> 7. Pie de Página (Footer): Copyright, enlaces secundarios y enlaces simulados a redes sociales.
>
> **[REQUISITOS TÉCNICOS Y ESTILO]**
> - Framework recomendado: Utiliza Tailwind CSS (vía CDN en el `<head>`) para garantizar un diseño estilizado, moderno y mobile-first sin necesidad de archivos CSS externos complejos.
> - Interactividad: Agrega animaciones suaves al hacer scroll y la lógica necesaria en JavaScript para que el menú móvil sea funcional (hamburguesa).
> - Componentes: Usa componentes visuales limpios, tipografías legibles (ej. Inter o Montserrat desde Google Fonts) y un esquema de colores coherente con la temática.
>
> **[RESTRICCIÓN CRÍTICA DE EJECUCIÓN]**
> Genera el código completo de extremo a extremo de forma autónoma. No dejes marcadores de posición vacíos como "// TODO:" o "...". El resultado debe estar listo para producción y ser auto-contenido para que funcione inmediatamente al abrirse en el navegador.

---

## Agentes y Modelos

| # | Agente | Modelo | Landing Page |
|---|---|---|---|
| 1 | `sdd-orchestrator` | `deepseek-v4-pro` | [`Opencode/index.html`](Opencode/index.html) |
| 2 | `Gemini` | `3.5 Flash (Medium)` | [`Antigravity/index.html`](Antigravity/index.html) |

---

## Capturas de Pantalla

### Portada Unificada

> *[Pendiente — capturar una vez deployado]*

### Landing Page — Agente 1 (sdd-orchestrator / deepseek-v4-pro)

> *[Pendiente — capturar secciones principales: Hero, Servicios, Contacto]*

### Landing Page — Agente 2 (Gemini / 3.5 Flash)

> *[Pendiente — capturar secciones principales: Hero, Servicios, Contacto]*

---

## Tecnologías Utilizadas

- **Tailwind CSS** — Framework utility-first vía CDN
- **Google Fonts** — Montserrat (headings) + Inter (body)
- **JavaScript Vanilla** — Interactividad sin dependencias externas
- **Intersection Observer API** — Animaciones al hacer scroll
- **Vercel** — Plataforma de deploy

---

## Conversación de Refinamiento

El prompt fue refinado a través de iteraciones sucesivas en Gemini para lograr una especificación clara y accionable:
[Ver conversación completa](https://gemini.google.com/share/eefb842d33f5)
