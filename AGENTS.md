# AGENTS.md — abi-2026-spanisch

Página interactiva de estudio para el Abitur de Español 2026 (NRW, Q2 Gk S). Sitio estático, **cero tooling**.

## Stack

Vanilla HTML/CSS/JS — sin build, sin dependencias, sin tests, sin linter, sin package.json. Abrir en navegador y listo.

## Archivos clave

| Archivo | Qué es |
|---------|--------|
| `index.html` | Página principal — 5 temas del examen con acordeón, progress tracker y timer |
| `tema5-monolog.html` | Práctica de monólogo para Tema 5 (Barcelona/Cataluña) — 8 diapositivas con solución docente |
| `img/*.jpeg` | Diapositivas extraídas del PDF de ejercicios |
| `Übungsmaterial_monolog-1.pdf` | PDF original de ejercicios (fuente de las imágenes) |
| `README.md` | Documentación completa para estudiantes (QR, instrucciones, temas) |

## Cómo trabajar

- No hay comandos de dev — los HTML se abren directo en el navegador
- No hay servidor, bundler, ni preprocesador
- No hay tests que correr
- `index.html` tiene todo el CSS y JS inline (~1500 líneas)
- `tema5-monolog.html` tiene su propio CSS y JS inline (~937 líneas)
- GitHub Pages deployea desde `main` — push a main publica automáticamente en `albecabrera.github.io/abi-2026-spanisch`

## Convenciones

- Commits: conventional commits (`feat:`, `fix:`, `docs:`)
- Contenido en alemán (público objetivo: estudiantes alemanes)
- Terminología del examen en español (temas, conceptos clave, vocabulario)
- No generar HTML, CSS, o JS nuevo a menos que se pida explícitamente
- Las imágenes en `img/` se usan solo en `tema5-monolog.html`; los JPEGs en raíz se usan en `index.html`
