# Análisis de Marketing y Rentabilidad de Clientes en Showz

**Autor:** Carlos Jaramillo  
**Rol:** Analista de Datos  

---

## 📌 Descripción del proyecto
Este proyecto analiza el comportamiento de los usuarios de **Showz**, una plataforma de venta de entradas para eventos, con el objetivo de optimizar los gastos de marketing.  
El análisis se basa en datos reales de visitas, pedidos y costos de adquisición entre enero de 2017 y diciembre de 2018, y busca determinar qué fuentes de marketing generan mayor rentabilidad y en qué momento los ingresos cubren el costo de adquisición de los clientes.

---

## 🎯 Objetivos
- Analizar cómo los usuarios interactúan con la plataforma.
- Identificar cuándo los usuarios comienzan a realizar compras.
- Calcular el valor que aporta cada cliente a la compañía (LTV).
- Evaluar los costos de adquisición de clientes por fuente de marketing.
- Determinar la rentabilidad de las inversiones en marketing (ROMI).
- Proporcionar recomendaciones estratégicas para la asignación del presupuesto de marketing.

---

## 🗂️ Descripción de los datos
El proyecto utiliza tres tablas principales:

- **visits**: registros del servidor con información sobre las visitas al sitio web.
- **orders**: información sobre los pedidos realizados por los usuarios.
- **costs**: datos de gastos diarios de marketing por fuente de adquisición.

### Columnas clave

**visits**
- `uid`: identificador único del usuario.
- `device`: dispositivo utilizado.
- `start_ts`: inicio de la sesión.
- `end_ts`: fin de la sesión.
- `source_id`: fuente de adquisición del usuario.

**orders**
- `uid`: identificador del usuario.
- `buy_ts`: fecha y hora de la compra.
- `revenue`: ingreso generado por el pedido.

**costs**
- `source_id`: identificador de la fuente de anuncios.
- `dt`: fecha.
- `costs`: gastos diarios de marketing.

---

## 🧪 Metodología

### 1. Preparación de datos
- Carga de datasets y revisión de la estructura.
- Conversión de columnas a los tipos de datos correctos.
- Creación de variables auxiliares para análisis temporal.
- Optimización de los datos para el cálculo de métricas.

### 2. Análisis de visitas
- Número de usuarios activos diarios, semanales y mensuales.
- Cantidad de sesiones por día.
- Duración de las sesiones.
- Frecuencia de retorno de los usuarios.

### 3. Análisis de ventas
- Tiempo transcurrido entre la primera visita y la primera compra.
- Número de pedidos por usuario en distintos períodos.
- Tamaño promedio de compra.
- Cálculo del valor del ciclo de vida del cliente (LTV).

### 4. Análisis de marketing
- Gastos totales y por fuente de adquisición.
- Costo de adquisición de clientes (CAC) por fuente.
- Retorno de la inversión en marketing (ROMI).
- Comparación de métricas por dispositivo y fuente de anuncios.
- Visualización de la evolución temporal de las métricas clave.

---

## 🛠️ Herramientas utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📊 Resultados y conclusiones
El análisis permite identificar qué fuentes de marketing generan clientes más rentables y en qué momento los ingresos superan el costo de adquisición.  
A partir de las métricas de LTV, CAC y ROMI, se formulan recomendaciones claras para optimizar la inversión en marketing y priorizar los canales con mejor desempeño.

---

## 📁 Estructura del repositorio
- `visits_log_us.csv`: registros de visitas al sitio.
- `orders_log_us.csv`: datos de pedidos.
- `costs_us.csv`: gastos de marketing.
- `Proyecto - Sprint 10.ipynb`: notebook con el análisis completo.
- `README.md`: documentación del proyecto.

---

## 👤 Autor
**Carlos Jaramillo**  
Analista de Datos