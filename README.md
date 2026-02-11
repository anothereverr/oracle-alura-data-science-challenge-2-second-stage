# 📊 Telecom X – Análisis y Predicción de Churn

## 1. Descripción del Proyecto

Este proyecto tiene como objetivo analizar el fenómeno de cancelación de clientes (*churn*) en Telecom X y desarrollar modelos predictivos que permitan identificar clientes con alta probabilidad de abandono.

A través de técnicas de análisis exploratorio de datos (EDA) y modelado supervisado, se busca comprender los factores que influyen en la cancelación del servicio y proponer estrategias accionables basadas en datos.

---

## 2. Objetivo

### Objetivo General
Desarrollar un modelo predictivo capaz de identificar clientes con riesgo de churn y analizar las variables que influyen en su cancelación.

### Objetivos Específicos
- Realizar limpieza y transformación de datos.
- Ejecutar análisis exploratorio para detectar patrones.
- Identificar variables relevantes asociadas al churn.
- Comparar modelos de clasificación.
- Proponer recomendaciones estratégicas basadas en evidencia.

---

## 3. Requisitos e Instalación

### Requisitos

- Python 3.9+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

## 4. Dataset

El dataset contiene información detallada de clientes de Telecom X, incluyendo variables demográficas, contractuales y de consumo del servicio.

### Principales variables:

- **Datos demográficos:** género, si es adulto mayor, si tiene pareja o dependientes.
- **Información contractual:** tipo de contrato (mensual, 1 año, 2 años).
- **Servicios contratados:** internet, fibra óptica, soporte técnico, seguridad online, streaming, entre otros.
- **Información financiera:** cargos mensuales y cargos totales.
- **Método de pago:** transferencia bancaria, tarjeta, electronic check, etc.
- **Antigüedad del cliente (tenure).**
- **Variable objetivo:** `Churn` (Sí / No).

El dataset fue sometido a:
- Limpieza de datos.
- Transformación de variables categóricas.
- Codificación para modelado.
- Escalamiento en caso necesario.

---

## 5. Gráficos

### Distribución de la Variable Churn
<img width="1549" height="676" alt="image" src="https://github.com/user-attachments/assets/99d46454-acb2-4bf2-989b-78310e785d70" />

### Correlación
<img width="916" height="918" alt="image" src="https://github.com/user-attachments/assets/807d24aa-9bf5-4ddb-af0c-10b22d7fbb74" />

### Heatmap
<img width="1151" height="893" alt="image" src="https://github.com/user-attachments/assets/f520d829-5e4f-4f5b-990e-1f6829fb7ac9" />

### Análisis dirigido: variables clave
<img width="1282" height="916" alt="image" src="https://github.com/user-attachments/assets/d2beb569-1ef3-4496-95ba-ce5157841c0b" />

### Scatter: cargo total vs meses de contrato
<img width="1492" height="891" alt="image" src="https://github.com/user-attachments/assets/b390bc03-6598-4b7c-8103-318d809e8805" />

### Matrices de confusión
<img width="1548" height="567" alt="image" src="https://github.com/user-attachments/assets/2f0ed1d6-c6db-4953-9dac-1fa58707e9b1" />

### Comparativa de metricas
<img width="1492" height="891" alt="image" src="https://github.com/user-attachments/assets/c493be24-9ecf-4a20-8ef1-efcfaa4a0267" />

### Coeficientes de regresión logistica
<img width="1142" height="913" alt="image" src="https://github.com/user-attachments/assets/66ac5233-fff4-4f4a-a783-a98701a98a6b" />

### Variables clave rendom forest
<img width="1142" height="916" alt="image" src="https://github.com/user-attachments/assets/41616a10-8817-44eb-a0d9-712589c7904c" />

---

## 6. Principales Hallazgos

- El churn representa aproximadamente una cuarta parte del total de clientes, lo que lo convierte en un problema relevante de negocio.
- Los clientes con menor antigüedad presentan significativamente mayor probabilidad de cancelación.
- Los contratos mensuales concentran la mayor tasa de churn, mientras que los contratos de 2 años presentan la menor.
- Los cargos mensuales elevados están correlacionados con mayor riesgo de abandono.
- Clientes que no cuentan con servicios adicionales (soporte técnico, seguridad online, streaming) muestran mayor probabilidad de churn.
- El método de pago "Electronic Check" presenta mayor asociación con cancelación.
- Los modelos predictivos (Regresión Logística y Random Forest) alcanzan un accuracy cercano al 78%, mostrando capacidad adecuada para identificar clientes en riesgo.

---

## 7. Conclusión

* El churn en Telecom X no es un fenómeno aleatorio, sino que responde a patrones estructurales identificables en los datos.

* El perfil de mayor riesgo corresponde a clientes nuevos, con contratos mensuales, altos cargos y sin servicios adicionales. En contraste, la fidelización aumenta con mayor antigüedad, contratos de largo plazo y mayor adopción de servicios complementarios.

* El modelo predictivo desarrollado permite anticipar cancelaciones y priorizar estrategias de retención basadas en evidencia.

* Implementar acciones focalizadas sobre clientes de alto riesgo puede reducir significativamente la tasa de churn, mejorar los ingresos recurrentes y aumentar el Customer Lifetime Value (CLV), permitiendo una gestión más estratégica y proactiva del negocio.
