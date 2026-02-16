# Plan de reorganización de series

## PythonistaMX — Serie `py`

### py1xx — Fundamentos de Python

| Nuevo # | Repo actual | Descripción |
|---------|-------------|-------------|
| py101 | py101 ✅ | Introducción a Python 3 |
| py111 | py111 ✅ | POO con Python 3 — extender con: Dataclasses, Type Hinting, Design Patterns básicos, Pythonic OOP |
| py121 | py121 ✅ | Refactorizar → Biblioteca estándar de Python (incluyendo async) |
| py131 | (nuevo) | Estructuras de Datos y Algoritmia Pythonica (Big-O, Grafos, Recursión) |
| py141 | (nuevo) | Automatización y Extracción de Datos con Python |

### py2xx — Desarrollo web con Python

| Nuevo # | Repo actual | Descripción |
|---------|-------------|-------------|
| py201 | py201 ✅ | Django |
| py211 | py211 ✅ | TDD con Python y Django |
| py221 | py221 ✅ | Flask |
| py241 | py241 ✅ | Diseño de APIs |
| py251 | py261 → renombrar | APIs asíncronas con SQLAlchemy y FastAPI |
| py261 | py401 → renombrar | DevOps para aplicaciones Python |

### py3xx — Ingeniería de datos

| Nuevo # | Repo actual | Descripción |
|---------|-------------|-------------|
| py311 | py311 ✅ | Fundamentos para Ingeniería de Datos |
| py321 | py541 → renombrar | Apache Airflow |
| py331 | *(nuevo)* | Pipelines con Apache Beam |
| py341 | *(nuevo)* | Spark y PySpark — base: py501 + py511 |
| py351 | *(nuevo)* | Buenas prácticas de Ingeniería de Datos |

### py4xx — Ciencia de datos *(todo nuevo)*

| # | Descripción | Base |
|---|-------------|------|
| py411 | Estadística y EDA | nuevo |
| py421 | ML con Scikit-learn | pyr101 + pyr105 |
| py431 | Deep Learning | nuevo |
| py441 | NLP | py301 notebooks 13-14 |
| py451 | Análisis de redes con NetworkX | py301 notebook 12 |

### py5xx — Big Data avanzado *(nivel especialización)*

> py341 cubre el nivel introductorio de Spark. py5xx asume ese conocimiento y profundiza.

| Nuevo # | Repo actual | Descripción |
|---------|-------------|-------------|
| py501 | py501 → refactorizar | PySpark avanzado: tuning, particionamiento, Spark internals |
| py511 | py511 → refactorizar | SparkSQL avanzado + Delta Lake en profundidad |
| py521 | *(nuevo)* | MLlib: Machine Learning distribuido a escala |
| py531 | *(nuevo)* | Structured Streaming: procesamiento en tiempo real |
| py551 | py551 ✅ | Fundamentos de Scala |
| py561 | *(nuevo)* | Spark con Scala |

### Acciones por repo

| Acción | Repos |
|--------|-------|
| ✅ Mantener número | py101, py111, py121, py201, py211, py221, py241, py311, py551 |
| 🔧 Refactorizar (mismo número, nuevo alcance) | py501 (intro→avanzado), py511 (intro→avanzado) |
| 🔄 Renombrar | py261→py251, py411→py131, py401→py261, py541→py321 |
| 📦 Archivar | py301, py321 (D3.js) |
| 🆕 Crear | py141, py331, py341, py351, py411–py451, py521, py531, py561 |
| 👤 Mover a personal | pyr101, pyr105, pycd101, pycd201 |

---

## Prioridades inmediatas

1. **py341** — mayor avance en planeación; base lista en py501 + py511
2. **py131** — Estructuras de Datos y Algoritmia (reemplaza plan anterior de Testing)
3. **py141** — Automatización y Extracción de Datos con Python
4. **py321** — renombrar py541 (Airflow); repo ya existe y está activo

---

## Cloudevel — Sin cambios estructurales

Las series `cd`, `gcp` y `az` ya son temáticas y consistentes.

### Pendientes

- Agregar descripciones a `cd101`, `az301`, `az421`
- Evaluar si hace falta `gcp201`
