# Análisis de Indicadores Clave de Rendimiento (KPIs) en Comercio Electrónico

Este repositorio contiene el desarrollo de una actividad práctica enfocada en el diseño, cálculo y visualización de Indicadores Clave de Rendimiento (KPIs) aplicados al comercio electrónico. El objetivo principal es demostrar cómo los Sistemas de Información de Gestión (MIS) transforman datos operativos crudos en conocimiento estratégico para la toma de decisiones gerenciales.

---

## Estructura del Proyecto

### Parte 1: Análisis de Datos Sintéticos (M-Commerce vs. E-Commerce)
En esta primera sección, se simula la salida de un Sistema de Procesamiento de Transacciones (TPS) mediante la generación de un dataset aleatorio utilizando `NumPy` y `Pandas`. 

* **Objetivo:** Determinar cuantitativamente si la estrategia de **M-Commerce (App Móvil)** es más rentable que el **E-Commerce tradicional (Web Desktop)**.
* **KPIs Evaluados:**
  1. **Ingresos Totales por Canal:** Medición de la rentabilidad absoluta de cada plataforma.
  2. **Ticket Promedio por Canal:** Valor medio de consumo por transacción para identificar el comportamiento del gasto.
  3. **Volumen de Transacciones:** Cantidad de ventas cerradas para evaluar la adopción y el tráfico de conversión.
  4. **Ingresos por Canal y Categoría:** Desglose detallado para identificar qué tipo de productos rinden mejor en cada entorno.

### Parte 2: KPIs para E-Commerce (Logística, Finanzas y CX)
Esta segunda sección trabaja sobre un conjunto de datos estructurado de una tienda electrónica (`ecommerce.zip`) y profundiza en tres pilares esenciales de la administración de operaciones:

1. **Gestión de Logística y Operaciones (Shipment & Warehouse):**
   * Evaluación de la eficiencia en la distribución física.
   * Análisis del costo promedio según el modo de transporte (avión, barco, carretera).
   * Monitoreo del volumen de ocupación (tanto en cantidad de unidades como en masa total en kilogramos) por bloque de bodega.
   * Optimización del peso de los paquetes distribuidos por canal de envío.

2. **Gestión Comercial y Financiera (Sales & Revenue):**
   * Determinación del ingreso bruto global de la organización.
   * Evaluación del impacto de la estrategia promocional mediante el análisis de descuentos otorgados cruzados con el nivel de fidelización del cliente.
   * Análisis de márgenes teóricos comparando el costo y el descuento respecto a la importancia asignada al producto.

3. **Experiencia y Fidelización del Cliente (Customer Experience - CX):**
   * Monitoreo del Índice de Satisfacción del Cliente (CSAT) segmentado por infraestructura logística (bloques de bodega).
   * Cálculo de la Tasa de Retención para clasificar la base de datos entre clientes nuevos y recurrentes.
   * Medición de la carga del soporte post-venta analizando la cantidad promedio de llamadas según la calificación otorgada por el usuario.

* **Procesamiento de Datos (Back-End):** Uso exclusivo de la librería `Pandas` para la manipulación masiva de datos y agrupaciones numéricas rápidas mediante operaciones vectorizadas (`.groupby()`, `.mean()`, `.sum()`). Las salidas técnicas de consola se limpiaron omitiendo metadatos redundantes para una lectura ejecutiva.
* **Visualización de Datos (Front-End):** Uso de `Matplotlib` para generar gráficos de barras simples, barras agrupadas y diagramas de pastel. Los gráficos están diseñados para una interpretación gerencial inmediata, aplicando transformaciones de unidades (como gramos a kilogramos) y escalas normalizadas.
