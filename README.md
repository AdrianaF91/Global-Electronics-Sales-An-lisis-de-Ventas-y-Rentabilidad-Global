# 📊 Global Electronics Sales — Análisis de Ventas y Rentabilidad Global

![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-Business_Intelligence-blue?style=for-the-badge)

## 🎯 Objetivo del Proyecto
Evaluar el desempeño comercial, la distribución geográfica y la rentabilidad del catálogo de una empresa global de venta de productos tecnológicos (*Global Electronics Retail*) entre **enero de 2016 y febrero de 2021**. El tablero está diseñado para que perfiles ejecutivos y operativos (Gerencia General, Operaciones, BI y Producto) identifiquen categorías críticas, optimicen márgenes de ganancia y respalden la toma de decisiones estratégicas.

🔗 **[Ver Dashboard Interactivo en Tableau Public](https://public.tableau.com/views/ProyectoFinal-Folcher/Portada)** 

---

## 📈 KPIs Principales Analizados
* **Ventas Totales:** $4.320.293.617
* **Ganancia Total:** $2.053.847.384
* **Margen de Ganancia Global:** 47,5%
* **Clientes Únicos:** 11.887 (50,7% Masculino | 49,3% Femenino)
* **Pedidos Únicos:** 26.326
* **Catálogo Activo:** 2.517 productos

---

## 🗂️ Fuente de Datos y Modelado
* **Dataset:** *Global Electronics Retail* (obtenido de Kaggle).
* **Arquitectura Relacional (Esquema Estrella):**
  * **Tabla de Hechos:** `Sales` (transacciones de ventas).
  * **Tablas de Dimensiones:** `Products` (vía `ProductKey`), `Customers` (vía `CustomerKey`) y `Stores` (vía `StoreKey`).
* **Cobertura:** Más de 15 atributos que combinan series temporales, datos demográficos, geolocalización y métricas financieras.

---

## 🛠️ Características Técnicas en Tableau
Para lograr un tablero dinámico y escalable se implementaron funcionalidades avanzadas de visualización y lógica de negocio:
* **Parámetro Dinámico (`Selección de Métrica`):** Permite al usuario alternar en tiempo real entre *Ventas Totales*, *Ganancia* y *Pedidos Únicos* en los gráficos principales.
* **Campos Calculados y Expresiones LOD (*Level of Detail*):** Cálculo preciso de margen de ganancia porcentual, conteo distintivo de clientes/pedidos y agregaciones por jerarquía de producto.
* **Navegación Multivista (3 Dashboards):**
  1. **Dashboard Ejecutivo (Clientes y Productos):** Mapa coroplético/burbujas de ventas por país, serie temporal (2016–2021), distribución por género y ranking por categoría/subcategoría.
  2. **Análisis de Rentabilidad:** Matriz de dispersión (*Ventas Totales vs. Ganancia*), Ranking Top 10 productos, heatmap de márgenes por subcategoría y matriz detallada a nivel SKU.
  3. **Documentación y Glosario:** Ficha técnica del modelo de datos, definición de métricas, conclusiones ejecutivas y glosario de términos BI.

---

## 💡 Principales Hallazgos e Insights
1. **Alertas en Categorías Deficitarias:**
   * Las subcategorías **Washers & Dryers (-235,6%)** y **Televisions (-42,7%)** presentan márgenes marcadamente negativos debido a referencias con costos operativos sin ingresos asociados o políticas de precios desajustadas, requiriendo auditoría inmediata.
   * **Projectors & Screens** muestra un margen crítico del **4,1%**, muy por debajo del promedio de la compañía (47,5%).
2. **Motores de Facturación y Estacionalidad:**
   * **Estados Unidos** lidera ampliamente el mercado (5.706 clientes), seguido por **Reino Unido** (1.570), **Canadá** (1.179) y **Alemania** (1.150).
   * La línea de computadoras de escritorio (*Desktops*), encabezada por los modelos **WWI Desktop PC2.33** y **Adventure Works Desktop**, concentra el mayor volumen de facturación individual.
   * Se observa un crecimiento sostenido entre 2018 y principios de 2020 (con picos estacionales marcados en fin de año), seguido de una contracción abrupta durante 2020.
3. **Oportunidades de Expansión:**
   * Categorías como **Monitors (62,6%)**, **Digital SLR Cameras (61,8%)**, **Movie DVD (61,0%)** y **Microwaves (59,1%)** mantienen márgenes altamente saludables, representando oportunidades clave para campañas de *cross-selling* y mayor inversión comercial.

---

## 🖼️ Vista Previa del Dashboard

```markdown
<img width="1799" height="799" alt="dashboard_ejecutivo" src="https://github.com/user-attachments/assets/89a7c07a-34e8-4c9c-a28b-547d6be24e1d" />
<img width="1799" height="799" alt="dashboard_rentabilidad" src="https://github.com/user-attachments/assets/c049fb7f-21f7-43dc-80d8-5ab27b05bbcb" />


