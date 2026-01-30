# Analyzing Gamezone's Revenue Drivers and Marketing Efficiency

# Project Background
**Gamezone**, fundada en 2018, es una empresa global de comercio electrónico especializada en la venta de productos de videojuegos nuevos y reacondicionados. Opera principalmente a través de su sitio web y aplicación móvil, atendiendo a clientes en múltiples regiones del mundo. El modelo de negocio se centra en la venta directa al consumidor, con un enfoque en productos populares de gaming como consolas, accesorios y equipos especializados.

Como analista de datos interno en Gamezone, se me ha asignado la tarea de analizar el rendimiento de productos e inventario para apoyar las decisiones estratégicas del equipo de Producto y Operaciones. Los objetivos clave del negocio incluyen:

- **Optimización de inventario:** Identificar qué productos generan la mayor parte de los ingresos para priorizar el stock
- **Estrategia de precios:** Comprender el valor promedio por pedido por producto
- **Expansión geográfica:** Identificar regiones con mayor potencial para productos específicos
- **Eficiencia operativa:** Analizar patrones temporales para planificar compras y logística

The SQL queries used to inspect and clean the data for this analysis can be found here [link].

Targed SQL queries regarding various business questions can be found here [link].

An interactive Tableau dashboard used to report and explore sales trends can be found here [link].



# Data Structure & Initial Checks

Gamezone's order data is housed in a single table, ```gamezone_orders_data``` containing 21,864 records, with each record representing a unique line item on a customer order.

The core metrics driving business analysis are:

- ```usd_price```: The monetary value of each transaction.
- ```purchase_ts``` and ```ship_ts```: Timestamps used to calculate sales trends and operational efficiency metrics.

The key dimensions for segmenting and analyzing these metrics include:

- ```product_name``` and ```product_id```: For product performance analysis.
- ```purchase_platform```: To distinguish user behavior between the Mobile App and Online Store.
- ```marketing_channel```: For attributing revenue and evaluating channel effectiveness.
- ```country_code```: For geographical sales analysis.

```gamezone_orders_data```
| Column Name | Data Type |
| ----: | :---|
| user_id | String |
| order_id | String |
| purchase_ts | Date |
| ship_ts | Date |
| product_name | String |
| product_id | String |
| usd_price | Float |
| purchase_platform | String |
| marketing_channel | String |
| account_creation_method | String |
| country_code | String |

The data spans from 2019 to 2021, enabling a comprehensive review of annual and seasonal trends.

Prior to analysis, the dataset underwent a rigorous validation and cleaning process to address inconsistencies in date formats, categorical values, and missing data, ensuring the reliability of all subsequent insights. The SQL queries used for inspection and quality control can be found here.

# Executive Summary

### Overview of Findings

Explain the overarching findings, trends, and themes in 2-3 sentences here. This section should address the question: "If a stakeholder were to take away 3 main insights from your project, what are the most important things they should know?" You can put yourself in the shoes of a specific stakeholder - for example, a marketing manager or finance director - to think creatively about this section.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Category 1:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 1]


### Category 2:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 2]


### Category 3:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 3]


### Category 4:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 4]



# Recommendations:

Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following: 

* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)
