# 🌐 Informe Final: Análisis de Evasión de Clientes en Telecom X

## 🚀 1. Resumen Ejecutivo

**Empresa:** Telecom X\
**Problema:** Alta tasa de cancelación de clientes (churn)\
**Objetivo:** Identificar factores asociados a la cancelación para diseñar estrategias de retención y apoyar el desarrollo de modelos predictivos.

### 🛠️ Metodología

- Importación de datos
- Limpieza y tratamiento de variables
- Análisis Exploratorio de Datos (EDA)
- Visualización de patrones
- Análisis de correlación

### 📊 Resultados Relevantes

- **Distribución de cancelaciones:** 25.7% de clientes desistieron.
- **Perfil de mayor riesgo:** Jóvenes, sin pareja, sin dependientes, que usan factura electrónica.
- **Tipo de contrato mensual** y **método de pago Electronic Check**: alto desistimiento.
- **Clientes con facturas más altas** y **menos meses de contrato** cancelan más.

### 🔹 Recomendaciones Clave

- Incentivar contratos anuales/bianuales.
- Segmentar clientes de riesgo para acción personalizada.
- Optimizar experiencia de pago electrónico.
- Desarrollar modelos de predicción de cancelación.

---

## 📊 2. Análisis Detallado y Gráfico

### 📉 2.1 Distribución General del Churn

- Total de clientes: 7267
- Activos: 71.2% (5174)
- Cancelados (De Baja - Desistieron): 25.7% (1869)
- Estado desconocido: 3.08% (224)

![alt text](imagenes_word/image.png)

**Conclusión:** hay una tasa considerable de cancelación que amerita análisis detallado.

### 👤 2.2 Variables Binarias (Perfil del Cliente)

- **Adulto Mayor:** tasa de cancelación del 22.9% vs 40.3% en no adultos mayores.
- **Pareja:** sin pareja = 32% de churn; con pareja = 19%.
- **Dependientes:** sin dependientes = 30.3% vs 14.9% con dependientes.
- **Factura Electrónica:** 32.5% de churn vs 15.9% en factura física.

![alt text](imagenes_word/image26.png)

![alt text](imagenes_word/image27.png)

![alt text](imagenes_word/image28.png)

![alt text](imagenes_word/image29.png)

![alt text](imagenes_word/image30.png)


**Hallazgo:** el perfil de mayor riesgo combina juventud, soltería, ausencia de dependientes y preferencia digital.

### 🛂 2.3 Variables Categóricas

- **Género:** tasa similar (26.1% mujeres, 25.3% hombres).
- **Tipo de internet:** Fibra óptica con 40.6% de cancelaciones.
- **Tipo de contrato:**
  - Mensual: 41.3%
  - 1 año: 3%
  - 2 años: 1.9%
- **Método de pago:**
  - Electronic Check: 43.8%
  - Otros métodos: 18% - 25%

![Método de pago](imagenes_word/image31.png)

![Método de pago](imagenes_word/image32.png)

![Método de pago](imagenes_word/image33.png)

![Método de pago](imagenes_word/image34.png)

![Método de pago](imagenes_word/image35.png)

**Hallazgo:** La suscripción del servicio de internet con fibra óptica están presentando una alta tasa de desistimiento, los contratos mensuales y el metodo de pagos electrónicos se asocian a mayor churn.

### 📊 2.4 Evasión asociada a Suscripciónes

![Suscripción](imagenes_word/image36.png)

6361 clientes tienen suscripción al servicio Telefonico, es la mayor base de suscripciones por servicio, pero de igual forma es el servicio que tienen mas desistimiento con 1699 clientes. Sigue luego la suscripción al servicio de Internet con una base de 6930 clientes, donde la opción de Fibra Optica tiene alto desistimiento con 1297 clientes.  

### 📊 2.5 Evasión asociada a facturación

#### ▶ Meses\_Contrato:

- Clientes cancelan en los primeros meses.
- Activos tienen mayor mediana y mayor dispersión.

![Boxplot Meses de Contrato](imagenes_word/image37.png)

#### ▶ Factura\_Mensual:

- Mediana más alta en clientes que cancelan.
- Cancelaciones concentradas entre cierto rango de valor mensual.

![Boxplot Factura Mensual](imagenes_word/image38.png)

#### ▶ Cargos\_Totales:

- Clientes activos acumulan más.
- Cancelaciones asociadas a menores montos acumulados (menos meses).

![Boxplot Cargos Totales](imagenes_word/image39.png)

#### ▶ Cuenta\_Diaria:

- los clientes que se dieron de baja tienden a tener un costo diario promedio (mediana) ligeramente superior en comparación con los clientes activos.
- Mediana más alta en clientes que cancelan.

![Boxplot Cuenta Diaria](imagenes_word/image40.png)



### 🔄 2.5 Análisis de Correlación

#### ▶ Variables con correlación negativa con cancelación:

- **Meses\_Contrato**: mayor antigüedad, menor churn.
- **Cargos\_Totales**: se relaciona con tiempo de servicio.

#### ▶ Variables con correlación positiva:

- **Factura\_Mensual**: clientes con cargos altos cancelan más.
- **Cuenta\_Diaria**: tendencia similar a factura.

#### ▶ Variables con correlación débil o nula:

- Algunas variables categóricas como el número de servicios contratados muestran baja relación lineal directa.

![Heatmap de correlación](imagenes_word/image25.png)

---

## 📈 3. Conclusiones Finales

- El perfil más vulnerable al churn incluye: clientes jóvenes, sin pareja ni dependientes, con contrato mensual y factura electrónica.
- La antigüedad y el tipo de contrato son los predictores más fuertes de cancelación.
- El tipo de servicio (fibra) y el método de pago también tienen impacto significativo.

## 🔹 4. Recomendaciones Finales

- Incentivar contratos a largo plazo.
- Mejorar experiencia de cliente en pagos digitales.
- Aplicar segmentación para acción temprana en clientes de riesgo.
- Integrar variables clave en modelos de predicción.

---

**Elaborado por:** Bibiana Trujillo Cedeño\
**Programa:** ONE + Alura LATAM\
**Especialización:** Ciencia de Datos

