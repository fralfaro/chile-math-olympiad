# CLAUDE.md — chile-math-olympiad

## Contexto del proyecto

Este repositorio contiene material de estudio para **olimpiadas matemáticas**,
basado en el libro oficial de la Olimpiada Nacional de Matemáticas de Chile:

> *Matemática y Olimpíadas*, Sociedad de Matemáticas de Chile (Somachi), Santiago 1994

El objetivo es un sitio educativo en **Quarto Book + GitHub Pages** dirigido a
estudiantes de enseñanza media y universitaria que quieran prepararse para la
Olimpiada Nacional de Matemáticas (OMC), IMO e Iberoamericana.

- **URL esperada:** `fralfaro.github.io/chile-math-olympiad`
- **Repositorio:** `https://github.com/fralfaro/chile-math-olympiad`
- **Origen del material:** copiado desde `fralfaro/academic-digital-skills`

---

## Estado actual del repositorio

> ✅ El material ya fue copiado desde `fralfaro/academic-digital-skills`.
> **No es necesario crear nada desde cero.**
> Tu tarea es **eliminar, renombrar y transformar** lo que existe.

Estructura actual (copiada):

```
chile-math-olympiad/
├── .github/
├── assets/
├── material/
│   ├── 00_intro/
│   ├── 01_github/
│   ├── 02_colab/
│   ├── 03_latex/
│   └── 04_quarto/
├── slides/
│   ├── .quarto/
│   ├── 00_intro/
│   ├── 01_github/
│   ├── 02_colab/
│   ├── 03_latex/
│   └── 04_quarto/
├── CLAUDE.md
├── _quarto.yml
├── custom.scss
├── dark.scss
├── index.qmd
├── light.scss
├── render_slides.py
└── requirements.txt
```

Estructura objetivo a alcanzar:

```
chile-math-olympiad/
├── .github/
│   └── workflows/
│       └── publish.yml        ← conservar
├── assets/                    ← conservar
├── material/
│   ├── 00_historia/
│   │   ├── index.qmd
│   │   ├── 01_mundial.qmd
│   │   ├── 02_chile.qmd
│   │   └── 03_medallistas.qmd
│   ├── 01_teoria_numeros/
│   │   ├── index.qmd
│   │   ├── 01_teoria.qmd
│   │   ├── 02_ejemplos.qmd
│   │   └── 03_problemas.qmd
│   ├── 02_induccion/
│   │   ├── index.qmd
│   │   ├── 01_teoria.qmd
│   │   ├── 02_ejemplos.qmd
│   │   └── 03_problemas.qmd
│   ├── 03_combinatoria/
│   │   ├── index.qmd
│   │   ├── 01_teoria.qmd
│   │   ├── 02_ejemplos.qmd
│   │   └── 03_problemas.qmd
│   ├── 04_analisis/
│   │   ├── index.qmd
│   │   ├── 01_teoria.qmd
│   │   ├── 02_ejemplos.qmd
│   │   └── 03_problemas.qmd
│   ├── 05_geometria/
│   │   ├── index.qmd
│   │   ├── 01_teoria.qmd
│   │   ├── 02_ejemplos.qmd
│   │   └── 03_problemas.qmd
│   ├── 06_problemas_resueltos/
│   │   └── index.qmd
│   └── 07_problemas_propuestos/
│       └── index.qmd
├── slides/
│   ├── 00_historia/
│   ├── 01_teoria_numeros/
│   ├── 02_induccion/
│   ├── 03_combinatoria/
│   ├── 04_analisis/
│   ├── 05_geometria/
│   ├── 06_problemas_resueltos/
│   └── 07_problemas_propuestos/
├── CLAUDE.md
├── _quarto.yml                ← reemplazar completo
├── dark.scss                  ← conservar
├── index.qmd                  ← reemplazar completo
├── light.scss                 ← conservar
├── render_slides.py           ← conservar
├── requirements.txt           ← conservar
└── README.md                  ← reemplazar completo
```

---

## Mapa de transformación

### Archivos raíz

| Archivo actual | Acción | Detalle |
|---|---|---|
| `_quarto.yml` | **REEMPLAZAR** | Ver sección `_quarto.yml objetivo` |
| `index.qmd` | **REEMPLAZAR** | Ver sección `index.qmd objetivo` |
| `README.md` | **REEMPLAZAR** | Ver sección `README.md objetivo` |
| `custom.scss` | **ELIMINAR** | No se usa |
| `dark.scss` | conservar | Sin cambios |
| `light.scss` | conservar | Sin cambios |
| `render_slides.py` | conservar | Sin cambios |
| `requirements.txt` | conservar | Sin cambios |

### Carpeta `material/`

| Carpeta actual | Acción | Carpeta final |
|---|---|---|
| `material/00_intro/` | **ELIMINAR contenido + RENOMBRAR** | `material/00_historia/` |
| `material/01_github/` | **ELIMINAR + RECREAR** | `material/01_teoria_numeros/` |
| `material/02_colab/` | **ELIMINAR + RECREAR** | `material/02_induccion/` |
| `material/03_latex/` | **ELIMINAR + RECREAR** | `material/03_combinatoria/` |
| `material/04_quarto/` | **ELIMINAR + RECREAR** | `material/04_analisis/` |
| *(no existe)* | **CREAR** | `material/05_geometria/` |
| *(no existe)* | **CREAR** | `material/06_problemas_resueltos/` |
| *(no existe)* | **CREAR** | `material/07_problemas_propuestos/` |

### Carpeta `slides/`

| Carpeta actual | Acción | Carpeta final |
|---|---|---|
| `slides/00_intro/` | **RENOMBRAR** (vaciar contenido) | `slides/00_historia/` |
| `slides/01_github/` | **RENOMBRAR** (vaciar contenido) | `slides/01_teoria_numeros/` |
| `slides/02_colab/` | **RENOMBRAR** (vaciar contenido) | `slides/02_induccion/` |
| `slides/03_latex/` | **RENOMBRAR** (vaciar contenido) | `slides/03_combinatoria/` |
| `slides/04_quarto/` | **RENOMBRAR** (vaciar contenido) | `slides/04_analisis/` |
| *(no existe)* | **CREAR** vacía | `slides/05_geometria/` |
| *(no existe)* | **CREAR** vacía | `slides/06_problemas_resueltos/` |
| *(no existe)* | **CREAR** vacía | `slides/07_problemas_propuestos/` |

> ⚠️ **`slides/` no se puebla con contenido en esta etapa.**
> Solo renombrar y dejar un `index.qmd` placeholder en cada subcarpeta.

---

## Contenidos por capítulo (1:1 con el libro Somachi)

### `00_historia/` — Introducción propia

| Archivo | Contenido |
|---|---|
| `index.qmd` | Qué son las olimpiadas, cómo usar este material, tabla de secciones |
| `01_mundial.qmd` | Historia de la IMO (1959→hoy), Putnam, Iberoamericana |
| `02_chile.qmd` | La OMC en Chile: Somachi, historia, organización actual |
| `03_medallistas.qmd` | Medallistas y participantes chilenos destacados en IMO |

### `01_teoria_numeros/` — Capítulo I

| Archivo | Contenido |
|---|---|
| `index.qmd` | Portada: objetivos, subtemas, referencia al libro |
| `01_teoria.qmd` | Divisibilidad · MCD/MCM · Coprimos · Primos · Congruencias · Aritmética modular · Ecuaciones Diofánticas · Funciones aritméticas |
| `02_ejemplos.qmd` | Ejemplos resueltos del libro (sección I.3) |
| `03_problemas.qmd` | Problemas de práctica con soluciones colapsadas + problemas OMC/IMO reales |

### `02_induccion/` — Capítulo II

| Archivo | Contenido |
|---|---|
| `index.qmd` | Portada: objetivos, subtemas |
| `01_teoria.qmd` | Progresiones aritméticas y geométricas · Principio de inducción débil y fuerte · Variantes · Sucesiones de Fibonacci |
| `02_ejemplos.qmd` | Ejemplos resueltos (secciones II.3 y II.4 del libro) |
| `03_problemas.qmd` | Problemas de práctica con soluciones colapsadas |

### `03_combinatoria/` — Capítulo III

| Archivo | Contenido |
|---|---|
| `index.qmd` | Portada: objetivos, subtemas |
| `01_teoria.qmd` | Principios combinatorios · Variaciones · Permutaciones (cíclicas, con repetición) · Combinaciones · Binomio de Newton · Pólya/Burnside · **Principio del Palomar** |
| `02_ejemplos.qmd` | Ejemplos resueltos (sección III.5 del libro) |
| `03_problemas.qmd` | Problemas de práctica con soluciones colapsadas |

### `04_analisis/` — Capítulo IV

| Archivo | Contenido |
|---|---|
| `index.qmd` | Portada: objetivos, subtemas |
| `01_teoria.qmd` | Números racionales y su orden · Números reales · Serie geométrica · Aproximaciones decimales · Representación en base $p > 1$ |
| `02_ejemplos.qmd` | Ejemplos resueltos (sección IV.4 del libro) |
| `03_problemas.qmd` | Problemas de práctica con soluciones colapsadas |

### `05_geometria/` — Capítulo V

| Archivo | Contenido |
|---|---|
| `index.qmd` | Portada: objetivos, subtemas |
| `01_teoria.qmd` | Conceptos básicos · Teoremas clásicos · Circunferencia · Baricentro · Incentro · Ortocentro · Circuncentro · Exinscritas · Ptolomeo · Carnot, Ceva, Menelao · Nueve puntos · Líneas de Euler y Simson |
| `02_ejemplos.qmd` | Ejemplos resueltos (sección V.13 del libro) |
| `03_problemas.qmd` | Problemas de práctica con soluciones colapsadas |

### `06_problemas_resueltos/` — Capítulo VI

| Archivo | Contenido |
|---|---|
| `index.qmd` | Problemas del Cap. VI (pág. 123–133) con soluciones detalladas paso a paso |

### `07_problemas_propuestos/` — Capítulos VII y VIII

| Archivo | Contenido |
|---|---|
| `index.qmd` | Problemas propuestos sin solución (Cap. VII) + "Fáciles de enunciar y difíciles de resolver" (Cap. VIII) |

---

## Reglas de contenido (aplicar a todos los `.qmd`)

### Público objetivo

- Estudiantes de 3° y 4° medio o primer año universitario
- Con base matemática de colegio, sin experiencia previa en olimpiadas

### Tono y redacción

- Lenguaje directo, preciso y motivador
- Rigor matemático completo: definiciones formales, demostraciones paso a paso
- Incluir motivación histórica antes de cada definición importante
- Estilo matemático estándar: "consideremos", "observemos", "demostramos que"

### Formato callouts

```markdown
::: {.callout-note title="Definición: Número primo"}
Un entero $p > 1$ es **primo** si sus únicos divisores positivos son $1$ y $p$.
:::

::: {.callout-tip title="Teorema: Infinitud de los primos (Euclides)"}
Existen infinitos números primos.

**Demostración:** ...
:::

::: {.callout-warning title="Ejemplo resuelto"}
**Problema:** ...
**Solución:** ...
:::
```

### Soluciones colapsadas en `03_problemas.qmd`

```markdown
**Problema 1.** Hallar todos los enteros $n$ tales que $n^2 + n + 41$ es primo.

::: {.callout-caution collapse="true" title="Ver solución"}
Para $n = 0, 1, \ldots, 39$ el resultado es primo.
Para $n = 40$: $40^2 + 40 + 41 = 41^2$, que no es primo.
:::
```

### Convenciones LaTeX

| Notación | Código |
|---|---|
| Divisibilidad $a \mid b$ | `$a \mid b$` |
| Congruencias $a \equiv b \pmod{n}$ | `$a \equiv b \pmod{n}$` |
| MCD $\gcd(a,b)$ | `$\gcd(a, b)$` |
| Combinaciones $\binom{n}{k}$ | `$\binom{n}{k}$` |
| Conjuntos $\mathbb{Z}, \mathbb{N}, \mathbb{R}$ | `$\mathbb{Z}$`, `$\mathbb{N}$`, `$\mathbb{R}$` |

### Cierre obligatorio de cada `03_problemas.qmd`

```markdown
## Problemas de competencias oficiales

**OMC [año] — Problema [N]:** [enunciado]

**IMO [año] — Problema [N]:** [enunciado]
```

---

## `_quarto.yml` objetivo

```yaml
project:
  type: book
  output-dir: docs
  render:
    - "index.qmd"
    - "material/00_historia/*.qmd"
    - "material/01_teoria_numeros/*.qmd"
    - "material/02_induccion/*.qmd"
    - "material/03_combinatoria/*.qmd"
    - "material/04_analisis/*.qmd"
    - "material/05_geometria/*.qmd"
    - "material/06_problemas_resueltos/*.qmd"
    - "material/07_problemas_propuestos/*.qmd"

book:
  title: "Matemática Olímpica"
  subtitle: "Preparación para la Olimpiada Nacional de Matemáticas de Chile"
  author: "Francisco Alfaro Medina"
  date: "2026"
  repo-url: "https://github.com/fralfaro/chile-math-olympiad"
  favicon: "assets/img/favicon.png"
  sidebar:
    logo: "assets/img/logo.png"

  chapters:
    - index.qmd
    - part: "Historia"
      chapters:
        - material/00_historia/index.qmd
        - material/00_historia/01_mundial.qmd
        - material/00_historia/02_chile.qmd
        - material/00_historia/03_medallistas.qmd
    - part: material/01_teoria_numeros/index.qmd
      chapters:
        - material/01_teoria_numeros/01_teoria.qmd
        - material/01_teoria_numeros/02_ejemplos.qmd
        - material/01_teoria_numeros/03_problemas.qmd
    - part: material/02_induccion/index.qmd
      chapters:
        - material/02_induccion/01_teoria.qmd
        - material/02_induccion/02_ejemplos.qmd
        - material/02_induccion/03_problemas.qmd
    - part: material/03_combinatoria/index.qmd
      chapters:
        - material/03_combinatoria/01_teoria.qmd
        - material/03_combinatoria/02_ejemplos.qmd
        - material/03_combinatoria/03_problemas.qmd
    - part: material/04_analisis/index.qmd
      chapters:
        - material/04_analisis/01_teoria.qmd
        - material/04_analisis/02_ejemplos.qmd
        - material/04_analisis/03_problemas.qmd
    - part: material/05_geometria/index.qmd
      chapters:
        - material/05_geometria/01_teoria.qmd
        - material/05_geometria/02_ejemplos.qmd
        - material/05_geometria/03_problemas.qmd
    - part: "Problemas"
      chapters:
        - material/06_problemas_resueltos/index.qmd
        - material/07_problemas_propuestos/index.qmd

lang: es

format:
  html:
    theme:
      light: [flatly, light.scss]
      dark: [darkly, dark.scss]
    number-sections: false
    toc: true
    page-layout: full
    html-math-method: mathjax
```

---

## `index.qmd` objetivo

```markdown
---
title: "Bienvenidos al curso!"
---

## Descripción

Este sitio es una guía de estudio para la preparación en **olimpiadas matemáticas**,
organizado siguiendo los capítulos del libro clásico de la Sociedad de Matemáticas
de Chile (Somachi):

> *Matemática y Olimpíadas*, Somachi, Santiago 1994.

Cubre los temas fundamentales de competencia: teoría de números, inducción matemática,
combinatoria, análisis elemental y geometría clásica. Cada capítulo incluye teoría
con demostraciones, ejemplos resueltos y problemas de práctica con soluciones.

## Capítulos

| # | Tema | Contenidos clave |
|---|---|---|
| 0 | Historia | La IMO, la OMC y el contexto chileno |
| I | Teoría de Números | Divisibilidad, primos, congruencias, aritmética modular |
| II | Inducción Matemática | Progresiones, Fibonacci, inducción fuerte |
| III | Combinatoria | Conteo, permutaciones, Binomio de Newton, Palomar |
| IV | Análisis | Racionales, reales, series, bases numéricas |
| V | Geometría | Triángulos, círculos, Ptolomeo, Ceva, Menelao |
| VI | Problemas Resueltos | Soluciones detalladas paso a paso |
| VII | Problemas Propuestos | Para practicar por tu cuenta |

## Referencia principal

::: {.callout-note title="Libro base"}
**Matemática y Olimpíadas**
Sociedad de Matemáticas de Chile (Somachi), Santiago 1994.

Disponible en: [www.olimpiadadematematica.cl](https://www.olimpiadadematematica.cl)
:::
```

---

## `README.md` objetivo

```markdown
# chile-math-olympiad

Material de estudio para olimpiadas matemáticas: teoría, ejemplos y problemas resueltos.

Basado en el libro *Matemática y Olimpíadas* (Somachi, 1994) y orientado a la
preparación para la Olimpiada Nacional de Matemáticas de Chile (OMC), la IMO
y competencias iberoamericanas.

## Contenidos

| Capítulo | Tema |
|---|---|
| 0 | Historia de las olimpiadas matemáticas |
| I | Teoría de Números |
| II | Inducción Matemática |
| III | Elementos de Combinatoria |
| IV | Elementos de Análisis |
| V | Elementos de Geometría |
| VI | Problemas Resueltos |
| VII | Problemas Propuestos |

## Sitio web

👉 [fralfaro.github.io/chile-math-olympiad](https://fralfaro.github.io/chile-math-olympiad)

## Referencias

- *Matemática y Olimpíadas*, Somachi, Santiago 1994
- [www.olimpiadadematematica.cl](https://www.olimpiadadematematica.cl)
- Cuadernos de Olimpiadas de Matemáticas, OMM (10 tomos)
- Hardy & Wright — *An Introduction to the Theory of Numbers*
- Apostol — *Introduction to Analytic Number Theory*
```

---

## Instrucción de inicio para Claude Code

Pega esto al abrir Claude Code en este repositorio:

```
Lee el CLAUDE.md completo antes de hacer cualquier cosa.

El material fue copiado desde fralfaro/academic-digital-skills.
Tu tarea es transformarlo siguiendo el mapa de transformación del CLAUDE.md.
No construyas desde cero — parte siempre de lo que existe.

Trabaja en este orden estricto:
1. Reemplazar _quarto.yml, index.qmd y README.md con el contenido del CLAUDE.md
2. Eliminar custom.scss
3. Transformar material/: renombrar carpetas según el mapa, recrear archivos internos
4. Transformar slides/: solo renombrar carpetas, dejar index.qmd placeholder en cada una
5. Poblar material/ sección por sección, empezando por 00_historia/

Antes de ejecutar cada paso muéstrame el plan detallado y espera mi confirmación.
```
