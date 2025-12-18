# 📂 Documentación de Datos (Dataset de Diagnóstico de Ventas)

Esta carpeta contiene la información técnica sobre las fuentes de datos utilizadas para el análisis de diagnóstico de la caída de ventas.

---

## 📊 Estructura del Modelo de Datos
El proyecto utiliza un **Modelo en Estrella (Star Schema)** con una tabla de granularidad intermedia para optimizar el rendimiento de las consultas DAX y facilitar la escalabilidad.

![Modelo de Datos en Estrella]([https://github.com/Elian-digital/Sales-Diagnosis-Churn-Analysis/blob/main/assets/data_model_schema.png?raw=true](https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/assets/data_model_schema.png))

El proyecto utiliza un **Modelo en Estrella (Star Schema)**...

### 1. Tablas de Hechos (Fact Tables)
* **`transactions`**: Es la tabla de hechos central que contiene el histórico de transacciones, importes (`amount`), fechas y geolocalización. Es la base para los cálculos de **Ingresos** y detección de transacciones declinadas.
* **`Pedidos`**: Actúa como tabla de vinculación (*bridge*) para conectar las transacciones con los productos específicos, permitiendo un análisis detallado a nivel de ítem.

### 2. Tablas de Dimensiones (Dimension Tables)
* **`Users`**: Contiene información demográfica y de comportamiento de los usuarios (Edad, Ciudad, País, Antigüedad). Incluye el campo `EstadoCliente` para segmentación avanzada.
* **`companies`**: Información geográfica y corporativa de las empresas cliente, incluyendo el canal de captación. Fundamental para identificar la fuga en el mercado de **Alemania**.
* **`products`**: Catálogo maestro con atributos como precio, color y peso. Se utilizó para confirmar la estabilidad de precios y validar la hipótesis del mix de ventas.
* **`Calendario`**: Tabla técnica generada para permitir el análisis de series temporales (YoY, MoM) y detectar patrones de estacionalidad.

---

## 🛠️ Procesos de Transformación (ETL)
Se aplicaron los siguientes pasos en **Power Query**:

1. **Gestión de Granularidad**: Desagregación y vinculación de pedidos para asegurar la correcta relación entre transacciones y productos.
2. **Limpieza de Datos Geográficos**: Tratamiento de nulos en coordenadas (`lat`, `longitude`) para garantizar la fiabilidad del análisis espacial.
3. **Optimización de Métricas**: Creación de columnas técnicas como `Amount_No_Declined` para aislar los ingresos reales de los intentos de pago fallidos.

---

## 📝 Nota sobre los Datos
Los datos utilizados en este proyecto son **sintéticos**, diseñados específicamente para validar la capacidad de diagnóstico ante la **"Paradoja del Ticket Promedio"**: el fenómeno donde el ticket medio sube mientras los ingresos caen debido al abandono de la base de clientes de volumen.
