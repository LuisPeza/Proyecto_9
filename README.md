# Proyecto 9: Optimización de Inversión en Marketing
> **Análisis de Negocio para Plataforma de Venta de Entradas (Ticketing)**

---

## 📋 Descripción del Proyecto
El objetivo principal es optimizar los gastos de marketing de una empresa de venta de entradas para eventos (similar a Ticketmaster). Mediante el análisis de registros de visitas, pedidos y gastos, se busca determinar la rentabilidad de los canales de adquisición y el comportamiento de compra de los usuarios.

### 🎯 Preguntas Clave de Negocio
* ¿Cómo interactúan los usuarios con el servicio?
* ¿Cuál es el tiempo promedio de conversión?
* ¿Cuál es el Valor de Vida del Cliente (LTV)?
* ¿Cuándo se alcanza el punto de equilibrio (Payback) de la inversión?

---

## 📂 Diccionario de Datos
El análisis integra tres fuentes principales de información:
1.  **Visitas:** Registros de sesiones (`Uid`, `Device`, `Start/End Ts`, `Source Id`).
2.  **Pedidos:** Transacciones financieras (`Uid`, `Buy Ts`, `Revenue`).
3.  **Gastos:** Costos de marketing por fuente y fecha (`source_id`, `dt`, `costs`).

---

## 📊 Métricas de Usuario y Visitas

### 👥 Análisis de Audiencia
El tráfico presenta una estacionalidad marcada, alcanzando su punto máximo al final del año.

| Periodo | Usuarios Únicos (Promedio) |
| :--- | :--- |
| **Mensual (MAU)** | Pico de **43,970** (Noviembre) |
| **Total Sesiones** | **228,169** usuarios únicos registrados |

### ⏱️ Duración de Sesiones
La duración de las sesiones varía significativamente, con varios registros de compra rápida (0-1 min) y otros de navegación extendida (18-28 min), lo que sugiere que algunos usuarios entran con una intención de compra directa mientras otros exploran eventos.

---

## 🛒 Análisis de Ventas y Conversión

### 🗓️ Tiempo de Conversión
Se observa una mejora en la agilidad de compra año tras año:
* **Promedio 2017:** 141.21 días para la primera compra.
* **Promedio 2018:** **100.68 días** para la primera compra.
* *Insight:* La plataforma ha logrado reducir el tiempo de decisión del cliente en un **28%**.

### 💸 Ticket Promedio y Volumen
* **Ingresos Totales:** $6,962,207.35
* **Número de Compras:** 761,807
* **Ticket Promedio:** **$9.14**



**Estacionalidad:** Diciembre de 2017 fue el mes récord con más de 100,000 pedidos, coincidiendo con festividades y eventos de fin de año. Por el contrario, junio presenta los niveles más bajos de actividad.

---

## 📣 Análisis de Marketing y Rentabilidad

### 💰 Inversión por Fuente
* **Inversión Total:** $329,131.62

| Fuente Id | Gasto Total | Costo Adquisición (CAC) | Evaluación |
| :--- | :--- | :--- | :--- |
| **Fuente 3** | $141,000+ | $1.89 | **Muy Costosa** |
| **Fuente 9** | $5,500 | **$0.59** | **Alta Eficiencia** |



### 📈 Retorno de Inversión (ROMI)
El **ROMI** general es de **159.5%**, lo que indica que por cada dólar invertido se generan 1.59 dólares. El valor de vida del cliente (**LTV**) se mantiene estable con un promedio de **$190**.

---

## 💡 Conclusiones y Recomendaciones Estratégicas

### 1. Optimización de Canales
* **Priorizar Fuentes 9 y 10:** Son las más eficientes. Tienen el CAC más bajo ($0.59) y un retorno de inversión saludable.
* **Reevaluar Fuente 3:** Es la que consume más presupuesto ($141k) con el CAC más alto ($1.89). Se recomienda reducir la inversión aquí y redistribuirla a canales más rentables.

### 2. Estrategia Estacional
* **Concentrar Presupuesto en Q4:** Octubre, noviembre y diciembre muestran la mayor demanda. Es vital aumentar la visibilidad en estos meses para capturar el pico de ventas.
* **Incentivos en Junio:** Dado que es el mes más bajo, se podrían lanzar campañas de fidelización o preventas exclusivas para reactivar la demanda estival.

### 3. Métricas Críticas para el Futuro
El enfoque debe mantenerse en el **LTV** y el **CAC**. Mientras el LTV ($190) sea significativamente superior al CAC ($0.59 - $1.89), el negocio es escalable y saludable.

---

## 🔗 Entregables
* [📂 Ver Análisis de Negocio Completo (Jupyter Notebook)](https://github.com/LuisPeza/Proyecto_9/blob/main/Proyecto_9_Analisis%20de%20negocio-%20Optimizar%20gastos%20marketing.ipynb)
