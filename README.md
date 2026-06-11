# ETL Básico con Power Query

## Descripción
Proyecto ETL desarrollado utilizando Excel y Power Query..

## Objetivo
Automatizar la extracción, transformación y carga de datos desde múltiples archivos CSV, 
sirviuendo para mejorar la productividad de procesos.

## Herramientas utilizadas
- Excel
- Power Query
- CSV Files

## Proceso ETL

### Extract
Importación de múltiples archivos CSV.

### Transform
- Limpieza de datos
- Conversión de tipos
- Creación de columnas calculadas

### Load
Carga automatizada hacia dashboard y tablas dinámicas.

## KPIs
- Ventas Totales
- Ventas por Ciudad
- Productos más vendidos

ETL
- automatización
- análisis de datos
- documentación
- uso de GitHub
- Power Query  

## 

Crear estructura del proyecto

PASO 1 — Crear carpeta en tu computadora

Nombre:

etl-powerquery-project

PASO 2 — Crear subcarpetas

Dentro crea:

Data
Processed_Data
Screenshots
Documentation
Estructura final
etl-powerquery-project
│
├── Data
├── Processed_Data
├── Screenshots
├── Documentation
└── README.md

PARTE 3 — Crear archivos CSV
PASO 1 — Abrir Excel

Usaremos datos ficticios de ventas.

PASO 2 — Crear archivo CSV #1

Guarda como:

ventas_enero.csv

Datos:

ID	Fecha	Cliente	Ciudad	Producto	Cantidad	Precio
1	01/01/2026	Juan	San Salvador	Laptop	1	800
2	03/01/2026	Ana	Santa Ana	Mouse	2	25

Guárdalo dentro de:

Data
PASO 3 — Crear archivo CSV #2

Guardar como:

ventas_febrero.csv

Datos:

ID	Fecha	Cliente	Ciudad	Producto	Cantidad	Precio
3	02/02/2026	Carlos	Soyapango	Monitor	1	200
4	05/02/2026	Sofia	La Libertad	Teclado	3	30

Guardar en:

Data
PARTE 4 — Crear archivo Excel ETL
PASO 1 — Crear Excel principal

Guardar como:

etl_process.xlsx
PASO 2 — Abrir Power Query

En:
Microsoft Excel

Ve a:

Datos → Obtener datos → Desde archivo → Desde carpeta

Selecciona:

Data
PASO 3 — Combinar archivos

Power Query detectará ambos CSV.

Presiona:

Combine & Transform

Aquí empieza el ETL.

PARTE 5 — TRANSFORM (Transformación)
PASO 1 — Limpiar columnas

Haz:

Remove blank rows
Remove duplicates
Cambiar tipos de datos
PASO 2 — Cambiar tipos
Columna	Tipo
Fecha	Date
Cantidad	Whole Number
Precio	Decimal Number
PASO 3 — Crear columna Total

Agregar columna → Columna personalizada

Nombre:

Total

Fórmula:

[Cantidad] * [Precio]
PASO 4 — Crear clasificación de ventas

Nueva columna:

Categoria_Venta

Fórmula:

if [Total] >= 500 then "Alta" else "Baja"
PASO 5 — Renombrar query

Lado izquierdo:

Cambiar nombre a:

Ventas_ETL
PARTE 6 — LOAD (Carga)
PASO 1 — Cargar datos

Presiona:

Close & Load

Excel creará una tabla limpia automáticamente.

PARTE 7 — Crear Dashboard básico
PASO 1 — Nueva hoja

Nombre:

Dashboard
PASO 2 — Insertar tabla dinámica

Insertar → Pivot Table

PASO 3 — Crear KPIs

Haz:

ventas totales
ventas por ciudad
productos más vendidos
ventas altas vs bajas
PASO 4 — Crear gráficos

Inserta:

gráfico de barras
gráfico circular
gráfico de líneas
PARTE 8 — Capturas para GitHub
PASO 1 — Tomar screenshots

Captura:

Power Query
Dashboard
Tabla final

Guardar en:

Screenshots
PARTE 9 — Subir proyecto a GitHub
PASO 1 — Entrar al repositorio

Dentro del repositorio:

Add file → Upload files
PASO 2 — Subir:
Excel
CSV
screenshots
PASO 3 — Editar README.md

Presiona:
✏️ Edit

Pega esto:

# ETL Básico con Power Query

