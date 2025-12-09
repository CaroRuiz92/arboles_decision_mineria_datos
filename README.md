# Trabajo Práctico N° 2 - Minería de Datos

## Aplicación de Técnicas de Minería de Datos en Problemas Reales

Este informe presenta la resolución del Trabajo Práctico N° 2 de Minería de Datos, cuyo objetivo es integrar los conocimientos adquiridos en las unidades 4 y 5, mediante la aplicación de diferentes algoritmos de Machine Learning (Regresión y Clasificación) en dos conjuntos de datos reales.

---

### Detalles de Entrega

* **Materia:** Minería de Datos
* **Año:** 2025
* **Formato de Entrega:** Archivo `.ipynb` (Jupyter Notebook)
* **Integrantes del Grupo:**
    * Ruiz, Carolina
    * Onega, Miranda
    * Quispe, Rocío

---

### Conjuntos de Datos Utilizados

Se trabajaron con dos conjuntos de datos:

1. **`1000_Companies.csv`**: Para el análisis del comportamiento financiero de 1000 empresas.
2. **`drug Type.csv`**: Para el análisis del tipo de droga farmacéutica.

---

### Resumen de las Actividades Realizadas

#### 1. Preprocesamiento General (Para ambos datasets)

* Realizar un Análisis Exploratorio de Datos (EDA): visualizar distribuciones, valores faltantes, correlaciones, etc..
* Limpiar el conjunto de datos (manejar valores faltantes, eliminar *outliers*) si es necesario.
* Codificar variables categóricas (si es necesario).
* Normalizar o estandarizar las características.

---

#### 2. Problema de Regresión: Estimación del Atributo `Profit`

* **Modelo:** Árboles de Decisión para Regresión.
* **Análisis de Parámetros:** Máximo profundidad, número mínimo de observaciones, número mínimo de observaciones por separación y criterio de separación.
* **Resultados:**
    * Graficar el árbol obtenido en el proceso de entrenamiento.
    * Mostrar los resultados sobre dos conjuntos de test utilizando:
        * Error Absoluto Medio (MAE).
        * Error Cuadrático Medio (MSE).
        * Raíz del Error Cuadrático Medio (RMSE).

---

#### 3. Problema de Clasificación: Estimación del Atributo `Droga`

**Preparación Adicional (Dataset `drug Type.csv`):**

* [cite_start]Generar dos conjuntos de datos para entrenamiento y evaluación, considerando las divisiones **80-20** y **70-30**.

**Modelos de Clasificación Implementados:**

| Modelo | Actividad Específica | Parámetros Analizados | Métricas de Evaluación (sobre ambos tests) |
| :--- | :--- | :--- | :--- |
| **Árboles de Decisión**  | Clasificación y aplicación de **poda**  | Máximo profundidad, mín. observaciones, mín. observaciones por separación, criterio de separación. | Precisión, Exhaustividad y Exactitud. |
| **Bayes Ingenuo**  | Discretización de atributos continuos (considerando un criterio de división). | Criterio de división para discretización. | Precisión, Exhaustividad y Exactitud. |
| **k-NN**  | | Cantidad de vecinos ($k$), Métrica y valor de $p$. | Precisión, Exhaustividad y Exactitud. |

---
