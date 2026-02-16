# py141: Automatización y Extracción de Datos con Python

Este curso representa la evolución moderna de la serie original de análisis de datos (`py121` legacy). Sirve como el puente fundamental entre la biblioteca estándar y la ingeniería de datos a escala, enfocándose en la obtención y validación del dato crudo.

## Enfoque

* **Pragmático:** Resolver problemas cotidianos de automatización (Excels pesados, PDFs, APIs lentas).
* **Moderno:** Stack actualizado (`httpx`, `Pydantic v2`, `SQLAlchemy 2.0`) reemplazando herramientas antiguas (`urllib`, `dicts` planos).

## Temario

### Módulo 1: Estructuración y Validación (El contrato de datos)
*De diccionarios caóticos a estructuras robustas.*

1. **01_modelado_con_dataclasses.ipynb**
   * Repaso breve de dataclasses vs dicts para estructuras de datos.
   * Inmutabilidad y tipado estático `frozen=True`.
2. **02_validacion_con_pydantic.ipynb**
   * Introducción a Pydantic v2 (`BaseModel`).
   * Validación de tipos, parsing robusto de datos sucios.
   * Serialización avanzada y `computed_fields`.

### Módulo 2: Interacción con la Web y APIs (Extract)
*El reemplazo asíncrono y robusto de `requests`.*

3. **03_cliente_http_moderno.ipynb**
   * Uso de `httpx`. Clientes síncronos vs asíncronos.
   * Manejo de reintentos, timeouts y autenticación (OAuth2 básico).
4. **04_consumo_avanzado_apis.ipynb**
   * Paginación automática.
   * Rate limiting (respetando los límites de la API).
   * Estrategias de caching de respuestas.

### Módulo 3: Formatos Documentales y No Estructurados (Scrape)
*Atacando problemas reales (ETLs de Excel, Web Scraping, PDFs).*

5. **05_web_scraping_eficaz.ipynb**
   * Automatización con `BeautifulSoup4` moderno y `Playwright` (en lugar de Selenium pesado).
   * Extracción de tablas HTML a estructuras de datos limpias.
6. **06_automatizando_excel.ipynb**
   * `openpyxl` y `xlsxwriter` para reportes automatizados.
   * Validación y limpieza de datos "dirty" en hojas de cálculo.
7. **07_mineria_de_documentos.ipynb**
   * Extracción inteligente de texto e información estructurada desde PDFs (`pdfplumber`).

### Módulo 4: Persistencia y Bases de Datos (Load)
*Del script al Data Lake o Warehouse.*

8. **08_dbapi_y_sqlite_avanzado.ipynb**
   * Entendiendo el DB-API 2.0 crudo (aprender lo que hay bajo el capó).
   * Funciones avanzadas de SQLite (JSON support en SQLite).
9. **09_sqlalchemy_core_2.0.ipynb**
   * SQL Expression Language (No ORM todavía).
   * Construcción de queries dinámicas y seguras.
   * Gestión de conexiones y Pools.
10. **10_sqlalchemy_orm_2.0.ipynb**
    * Mapeo moderno declarativo (`Mapped`, `mapped_column`).
    * Relaciones, cargas perezosas vs ansiosas (N+1 problem).
    * Patrón Repository para acceso a datos.

### Módulo 5: Pipelines y CLI (El pegamento)

*Orquestación ligera antes de Airflow/Prefect.*

11. **11_interfaces_de_linea_de_comandos.ipynb**
    * Creación de herramientas de ETL CLI con `Click` o `Typer`.
12. **12_logs_y_observabilidad_en_etl.ipynb**
    * Logging estructurado (JSON logs) para sistemas de producción.
    * Manejo de errores y alertas en pipelines de datos.
