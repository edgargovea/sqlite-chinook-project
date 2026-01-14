# Sales Analysis in a Relational Database (SQLite)

Proyecto de análisis de la base de datos relacional _Chinook_, enfocado en la exploración, consulta y análisis de información de ventas, clientes y productos musicales.

Se diseñaron y ejecutaron consultas SQL de complejidad creciente (JOINs, subconsultas y CTEs) para responder preguntas de negocio como ingresos por país, clientes más valiosos, desempeño por género musical y tendencias temporales.

El proyecto integra SQLite, SQL y Python (pandas, Jupyter) para análisis adicional y visualización, y documenta de forma clara la estructura de la base de datos y los resultados obtenidos.

<img src="figures/Ventas_por_pais.png" width="600">

---

##  Estructura de la Base de Datos Chinook

La base de datos **Chinook** modela una tienda de música digital. Incluye información sobre artistas, álbumes, géneros, clientes, facturas y más.  
A continuación, se describen sus tablas principales:

##  Chinook Database Structure
| Table          | Description                                 | Primary Key   |
| -------------- | ------------------------------------------- | ------------- |
| employees      | Company employees and reporting structure   | EmployeeId    |
| customers      | Customer profiles and assigned support reps | CustomerId    |
| invoices       | Sales invoices issued to customers          | InvoiceId     |
| invoice_items  | Line items for each invoice (tracks sold)   | InvoiceLineId |
| artists        | Music artists catalog                       | ArtistId      |
| albums         | Albums released by artists                  | AlbumId       |
| tracks         | Individual music tracks                     | TrackId       |
| genres         | Music genres                                | GenreId       |
| media_types    | Audio file formats                          | MediaTypeId   |
| playlists      | User-defined playlists                      | PlaylistId    |
| playlist_track | Bridge table between playlists and tracks   | —             |


---
 <img src="figures/Preduccion_Ventas.png" width="270"> <img src="figures/Ventas_por_genero.png" width="270">

## Objetivos del Proyecto

El objetivo general de este proyecto es **analizar y extraer valor de la base de datos relacional Chinook** mediante consultas SQL y análisis complementario en Python, simulando escenarios reales de análisis de negocio.

* Aplicar SQL y Python para explorar, consultar y analizar información de ventas, clientes y productos musicales, generando insights relevantes para la toma de decisiones.

####  Exploración y comprensión de la base de datos

* Comprender la **estructura relacional** de la base de datos Chinook.
* Identificar entidades clave, relaciones entre tablas y campos relevantes.
* Documentar el esquema y las tablas principales de forma clara y reproducible.

####  Desarrollo de consultas SQL

* Diseñar y ejecutar consultas SQL de **complejidad progresiva**:

  * Consultas básicas (SELECT, WHERE, GROUP BY).
  * Consultas intermedias con **JOINs múltiples**.
  * Consultas avanzadas con **subconsultas y CTEs**.
* Optimizar consultas para responder preguntas analíticas y de negocio.

####  Análisis de negocio y generación de insights

* Analizar métricas clave como:

  * Ingresos por país, cliente, género y artista.
  * Identificación de clientes más valiosos (*Customer Lifetime Value*).
  * Desempeño de ventas por período de tiempo.
* Responder preguntas de negocio reales basadas en datos.

####  Análisis y visualización de datos

* Integrar **SQLite con Python** para análisis adicional.
* Utilizar **pandas y Jupyter Notebooks** para:

  * Limpieza y transformación de datos.
  * Visualización de resultados mediante gráficos claros e interpretables.
  * Identificación de patrones y tendencias.

#### Comunicación y reproducibilidad

* Presentar los resultados de forma clara mediante:
  * Notebooks bien documentados.
  * Visualizaciones de resultados.

---
## 📌 Referencias  
- [SQLite Tutorial - Sample Database](https://www.sqlitetutorial.net/sqlite-sample-database/)  
- Documentación oficial de SQLite  

---
 <img src="figures/Generos_USAB.png" width="400">
