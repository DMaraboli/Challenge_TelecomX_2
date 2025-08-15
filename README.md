# Challenge_TelecomX_2
# 📊 Análisis de Cancelación de Clientes (Churn) en TelecomX

Este repositorio contiene un análisis completo para predecir la cancelación (*churn*) de clientes de la empresa ficticia **TelecomX**, utilizando un enfoque de **Machine Learning** con Python.  
El proyecto incluye **análisis exploratorio de datos (EDA)**, **preprocesamiento**, **modelado**, **optimización de hiperparámetros** y **evaluación de modelos**.

---

## 📂 Contenido del Proyecto

1. **Extracción y Preparación de Datos**  
   - Carga del dataset (`datos.csv`).  
   - Limpieza y eliminación de variables irrelevantes.  

2. **Análisis Exploratorio (EDA)**  
   - Distribución de `Churn` y variables categóricas.  
   - Análisis de variables numéricas (`tenure`, `Charges.Monthly`, `Cuentas_diarias`, etc.).  

3. **Ingeniería de Características**  
   - Creación de `Cuentas_diarias` como métrica robusta de gasto.  
   - Eliminación de variables redundantes y codificación *One-Hot*.  
   - Análisis de correlación y selección de features relevantes.  

4. **Balanceo de Clases**  
   - Uso de **SMOTE** para manejar el desbalance (73.46% permanece vs 26.54% cancela).  

5. **Modelado Inicial**  
   - Modelo base: **Regresión Logística**.  

6. **Comparación de Modelos**  
   - **Árbol de Decisión**  
   - **Random Forest**  
   - **KNN**  

7. **Importancia de Variables**  
   - Análisis con Random Forest para ranking de features.  

8. **Selección de Variables y Validación Cruzada**  
   - Evaluación con distintas cantidades de features.  

9. **Optimización de Hiperparámetros**  
   - **GridSearchCV** para maximizar *F1 Score*.  

10. **Evaluación Final**  
    - Métricas de rendimiento en datos de test.  
    - Matrices de confusión y métricas detalladas.

---

## 🛠️ Tecnologías y Librerías Usadas

- **Python 3.10+**
- **Pandas** — Manipulación y limpieza de datos.
- **NumPy** — Operaciones numéricas.
- **Matplotlib / Seaborn** — Visualización de datos.
- **Scikit-learn** — Modelado, métricas, validación cruzada.
- **Imbalanced-learn (SMOTE)** — Balanceo de clases.
- **Google Colab** — Entorno de ejecución.

---

## 📊 Resultados Clave

- **Random Forest** resultó ser el modelo con mejor equilibrio entre *Recall* y *Precision*.  
- Mantener entre **20 y 22 variables** optimiza el rendimiento sin pérdida significativa.  
- El *GridSearchCV* permitió mejorar las métricas optimizando la profundidad y número de estimadores.  

---

## 🚀 Ejecución del Notebook

1. Clonar este repositorio.
   
2. Abrir en Google Colab.

3. Subir el archivo datos.csv al entorno de Colab.

4. Ejecutar las celdas en orden.

---

## ✍️ Autor

Daniel Medina
