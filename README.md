# 📊 Dashboard de Ventas 2024–2025

## Descripción del proyecto
Este proyecto presenta un análisis exploratorio y visualización interactiva de datos de ventas correspondientes al período 2024–2025.

El objetivo fue transformar datos comerciales en información útil para apoyar la toma de decisiones, identificando tendencias de ventas, productos líderes, concentración de ingresos y desempeño por canal de venta.

El flujo de trabajo incluyó extracción de datos desde una API, análisis exploratorio en Python y construcción de dashboard interactivo en Power BI.

---

## Problema de negocio
Las organizaciones comerciales generan grandes volúmenes de datos de ventas, pero frecuentemente carecen de herramientas visuales que permitan responder preguntas clave como:

- ¿Cuál es la evolución mensual de ventas?
- ¿Qué productos generan mayor facturación?
- ¿Existe concentración de ingresos en pocos productos?
- ¿Qué canal de venta presenta mejor desempeño?

Este proyecto busca resolver estas preguntas mediante un dashboard analítico que facilite el monitoreo comercial.

---

## Objetivos
- Analizar comportamiento temporal de ventas.
- Identificar productos con mayor contribución económica.
- Aplicar análisis de Pareto (80/20) para detectar concentración de ingresos.
- Comparar desempeño entre canales de venta.
- Construir visualizaciones dinámicas e interactivas.

---

## Fuente de datos
Los datos fueron obtenidos mediante una **API pública**.

Información incluida:
- fecha
- producto
- categoría
- precio
- cantidad
- ingreso
- canal de venta
- año y mes

---

## Metodología

### 1. Extracción de datos
- Consumo de API para obtención de registros de ventas.
- Conversión a formato tabular para análisis.

### 2. Limpieza y transformación
Realizada en Python:
- revisión de valores faltantes
- validación de tipos de datos
- transformación de fechas
- generación de variables derivadas:
  - año
  - mes
  - nombre del mes
  - ticket promedio

### 3. Análisis exploratorio (EDA)
Desarrollado en Python:
- distribución de ventas
- tendencias temporales
- análisis por producto
- comparación entre canales
- identificación de patrones comerciales

Librerías utilizadas:
- pandas
- numpy
- matplotlib
- seaborn

### 4. Visualización
Dashboard construido en **Power BI** con:
- KPIs dinámicos
- gráfico de tendencia mensual
- ranking de productos
- gráfico de Pareto
- distribución por canal
- insights dinámicos mediante DAX

---

## Herramientas utilizadas
- Python
- Jupyter Notebook
- Power BI
- API REST

---

## Principales hallazgos
- Tendencia descendente en ventas durante el período analizado.
- Alta concentración de ingresos en pocos productos.
- Laptop HP como producto líder.
- Los 3 principales productos concentran aproximadamente 70% de ventas.
- Diferencias de desempeño entre canales online y tienda.

---

## Dashboard
Vista general del dashboard:

![Dashboard](dashboard.png)

---

## Estructura del proyecto
```bash
Proyecto_Ventas/
│
├── data/
│   └── ventas.csv
│
├── notebooks/
│   └── eda_ventas.ipynb
│
├── powerbi/
│   └── dashboard_ventas.pbix
│
└── README.md
