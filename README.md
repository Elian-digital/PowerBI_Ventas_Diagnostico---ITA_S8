
## 🚀 **Sales Diagnosis & Churn Analysis: Identifying Revenue Leakage | Proyecto End-to-End con Power BI (ITAcademy)**

Este proyecto es un **análisis de diagnóstico y estrategia *End-to-End*** que abordó la caída de ventas en un comercio online. El análisis aplicó habilidades avanzadas de **Modelado de Datos** y **Diseño de Información** para descubrir la causa raíz cuantificable: la pérdida masiva de clientes en el mercado alemán.

-----

## 🛠️ Stack Técnico y Metodología

* **Herramientas:** Power BI Desktop, Power Query, DAX.
* **Modelado:** Esquema en Estrella (Star Schema) con tablas de hechos y dimensiones estandarizadas.
* **ETL:** Limpieza de datos avanzada en Power Query (Tipado de datos, manejo de nulos y normalización de moneda).
* **Visualización:** Aplicación de principios de **Gestalt y Jerarquía Visual** para optimizar la carga cognitiva del usuario.

-----

### 💡 **El Desafío (La Crisis Comercial y el Punto Ciego)**

La dirección observaba una baja generalizada en los ingresos sin conocer el origen. El sistema de *reporting* previo carecía de la capacidad de segmentación y modelado para aislar factores críticos como la fuga de clientes.

  * **El Problema:** Determinar si la caída de ventas era un problema general de producto o un problema de retención en un mercado específico, para dirigir una acción estratégica inmediata.

-----

### 📖 **La Historia del Dato**

> "Este proyecto empezó con una simple pregunta: *¿Por qué están cayendo las ventas?* Al principio, no se sabía de donde venía esta caída. Tras hacerle unas cuantas preguntas a la Base de datos (qué, dónde, quién, cuándo) empezaron a salir pistas. Al centrar el foco en la geografía y las interacciones del cliente, el dashboard comenzó a 'hablar'. El punto de inflexión fue la segmentación por continente, donde la luz de alerta se encendió sobre **Alemania**. El análisis de las series de tiempo y los recuentos de clientes reveló que el problema no era de rendimiento de producto, sino de una **fuga masiva en una empresa en concreto**. Transformamos una vaga preocupación sobre 'ventas bajas' en el diagnóstico preciso de un problema de retención, proporcionando un *insight* que requería una intervención estratégica inmediata."

-----

### 🎯 **La Solución (Implementación Técnica y Descubrimiento)**

El proyecto se centró en la ingeniería de datos y el diseño para facilitar la exploración y el diagnóstico, sirviendo como una herramienta integral de *reporting* y análisis.

  * **Herramientas Clave:** Power BI Desktop (Modelado, DAX, Visualización) y Power Query (ETL/Limpieza).

#### 1\. Ingeniería y Modelado de Datos (Back-End)

  * **Modelo de Estrella Optimizado:** Se construyó un **Modelo de Estrella** robusto unificando las tablas de hechos (transacciones) y las dimensiones (clientes, productos, tiempo), incluyendo la creación de **tablas intermedias** para garantizar la integridad y la velocidad de las consultas.
  * **Limpieza de Datos Exhaustiva:** Implementación de **numerosos pasos de transformación** en Power Query (cambio de unidades, estandarización de formatos, manejo de inconsistencias) para garantizar la calidad y fiabilidad de los datos de origen.

    ## 📊 Métricas Implementadas (DAX)

Para este diagnóstico, desarrollé medidas personalizadas que permiten profundizar en el análisis:
* **Churn Rate Estimado:** Identificación de clientes sin transacciones en el último periodo.
* **Variación de Ingresos YoY:** Comparativa interanual para aislar el efecto de la estacionalidad.
* **Ticket Promedio Dinámico:** Calculado para contrastar con el volumen de pedidos y detectar el "Efecto Espejismo".

#### 2\. Análisis Exploratorio Multi-Dimensional

El dashboard fue diseñado para una exploración exhaustiva antes del diagnóstico, permitiendo al usuario descartar hipótesis mediante:

  * **Análisis de Portafolio:** Visualización de **qué vendemos** (productos, categorías) y su rendimiento.
  * **Análisis Geográfico y Logístico:** Exploración de **dónde vendemos** y el flujo de ventas.
  * **Análisis Temporal y de Estacionalidad:** Identificación de patrones de compra por **continente** y periodo.
  * **Análisis de Canales:** Evaluación de la contribución de los canales digitales, incluyendo las **redes más usadas**.

#### 3\. El Descubrimiento Crítico

  * **Diagnóstico Preciso:** El análisis basado en el modelo reveló que la pérdida de clientes se concentraba en **Alemania**, y esta fuga de clientes representó el **4% del total de ventas** del comercio.


### 🔍 Análisis de Diagnóstico: El "Efecto Espejismo" del Ticket Promedio

Un hallazgo crítico del proyecto fue la correlación inversa entre el Ticket Promedio y los Ingresos Totales a partir de 2022:

* **El Espejismo del Promedio:** Aunque los precios unitarios se mantuvieron estables, el Ticket Promedio aumentó significativamente. Esto no indica una mayor rentabilidad, sino la **pérdida masiva de clientes de volumen menor**.
* **Segmentación y Abandono:** Al desaparecer los clientes que realizaban compras pequeñas pero constantes, el promedio se desplazó hacia arriba debido a los pocos clientes "High-End" restantes. 
* **Diagnóstico de Negocio:** El comercio perdió su base de clientes masiva (especialmente en Alemania), reduciendo la salud del ecosistema y la frecuencia de compra. Esto sugiere que la competencia capturó el mercado de entrada, dejando a la empresa en una posición vulnerable con baja diversificación de clientes.


-----

### ✨ **Logros y Resultados (Valor y Perfil Profesional)**

  * **Impacto Cuantificable y Diagnóstico:** El análisis proporcionó un diagnóstico inmediato sobre la causa del problema, **cuantificando su impacto en el 4% de las ventas totales**, permitiendo enfocar los recursos hacia la retención de clientes en un mercado específico.
  * **Amplitud Analítica y Reporting Base:** El dashboard se consolidó como una **herramienta integral de *reporting*** que ofrece una visión completa de la estacionalidad, rendimiento de productos y eficacia de los canales digitales.
  * **Gobernanza y Calidad del Dato:** Se garantiza la fiabilidad del informe mediante la aplicación de **procesos rigurosos de limpieza y estandarización** en Power Query, asegurando que el informe sea una **Fuente Única de Verdad (SSOT)**.
  * **Visualización de Alto Impacto:** La presentación fue diseñada con una **alta atención al detalle gráfico (gracias al *background* de Diseñador Gráfico)**, empleando colores y jerarquías para guiar al usuario y **resaltar el segmento crítico**.

-----

## 📊 **Visualizaciones del Dashboard (Diseño de Información en Acción)**

El diseño gráfico se aplicó para transformar la data en un diagnóstico claro y visualmente intuitivo, demostrando la capacidad de comunicación de *insights*.

### Vista 1: Dashboard Principal (Vista Integral)

![Dashboard Power BI](Dashboard_1.png)

  * **Leyenda:** Demostración de la amplitud analítica, mostrando la visión general de ventas, estacionalidad y el impacto de las redes sociales, sirviendo como punto de partida para todas las exploraciones.

### Vista 2: El Descubrimiento Crítico
![El descubrimiento](empresas_alemania.png)

  * **Leyenda:** Gráfico que demuestra la caída en ventas de Alemania, validando el hallazgo crítico del proyecto.

### Vista 3: Clientes que desaparecen

![El descubrimiento](clientes.png)

  * **Leyenda:** Ilustra el uso de bloques blancos para visibilizar al gran cantidad de clientes de paises como Italia, Poland o Uk que desaparecieron.

-----

### ⏭️ **Próximos Pasos y Escalabilidad**

Este proyecto sienta las bases para futuras iniciativas de inteligencia de negocio, mostrando la visión estratégica del análisis:

  * **Monitoreo Activo:** Implementación de un sistema de alertas en Power BI Service para notificar inmediatamente sobre picos anormales en la tasa de abandono de clientes (Churn Rate).
  * **Análisis Predictivo:** Ampliación del modelo con datos externos o algoritmos para predecir qué clientes tienen mayor probabilidad de fuga en el futuro.
  * **Dashboard de Rentabilidad:** Desarrollo de un informe enfocado en el **Customer Lifetime Value (CLV)** para priorizar los esfuerzos de retención.

-----

## 🚀 Conclusiones y Visión Estratégica

1.  **Diagnóstico:** La caída de ventas no es un problema de producto, sino de **retención en la base de la pirámide**. El aumento del ticket promedio es un síntoma de la pérdida de clientes de bajo volumen.
2.  **Impacto:** El mercado alemán es el "early warning" de esta tendencia. Si no se actúa, el 4% de pérdida actual podría escalar a otros mercados europeos.
3.  **Próximos Pasos (Escalabilidad):** * Integrar un análisis de **Cohortes** para medir la retención por mes de adquisición.
    * Implementar un **Dashboard de Alerta Temprana** que detecte caídas de volumen por país antes de que afecten al ingreso global.

-----

### 🤝 **Contacto**

  * **Desarrollador:** Elian Daghoum
  * **Perfil de GitHub:** https://github.com/Elian-digital
  * **LinkedIn/Contacto:** https://www.linkedin.com/in/eliandaghoum/
