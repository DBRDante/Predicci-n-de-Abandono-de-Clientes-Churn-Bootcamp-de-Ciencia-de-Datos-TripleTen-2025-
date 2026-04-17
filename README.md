# Predicción de Abandono de Clientes – Beta Bank

## Problema
La pérdida de clientes (churn) es un problema crítico en el sector bancario, ya que impacta directamente en los ingresos.  
El objetivo de este proyecto es construir un modelo de machine learning capaz de predecir si un cliente abandonará el banco, permitiendo implementar estrategias de retención proactivas.

---

## Datos
El conjunto de datos contiene variables relacionadas con los clientes, tales como:

- **Datos demográficos:** edad, geografía, género  
- **Información de cuenta:** balance, antigüedad, número de productos  
- **Indicadores de actividad:** uso de tarjeta de crédito, membresía activa  

Los datos presentan **desbalance de clases**, lo que requirió técnicas adicionales de preprocesamiento.

---

## Enfoque
El proyecto siguió un flujo estructurado de trabajo en machine learning:

- Limpieza y preprocesamiento de datos  
- Análisis exploratorio de datos (EDA)  
- Ingeniería de variables  
- Entrenamiento y evaluación de modelos  

Se evaluaron varios modelos:

- Regresión Logística  
- Árbol de Decisión  
- Random Forest  

Para abordar el desbalance de clases, se aplicaron técnicas de **sobremuestreo (upsampling)** y **submuestreo (downsampling)**.

---

## Resultados
El modelo con mejor desempeño fue **Random Forest con sobremuestreo**, obteniendo:

- **F1 Score:** 0.626  
- **ROC AUC:** 0.856  

### Otros resultados relevantes:
- Random Forest (base): F1 = 0.601, ROC AUC = 0.850  
- El submuestreo mejoró el recall pero redujo la precisión  
- La Regresión Logística mostró un desempeño inferior  
- Los Árboles de Decisión tuvieron resultados intermedios, pero menor estabilidad que métodos de ensamblado  

La curva ROC mostró una buena capacidad de clasificación, indicando un equilibrio adecuado entre verdaderos positivos y falsos positivos.

---

## Conclusión
El modelo **Random Forest con sobremuestreo** demostró ser el más adecuado para predecir el abandono de clientes. Logró el mejor equilibrio entre precisión y recall, manteniendo una sólida capacidad de discriminación.

Este modelo representa una solución robusta para problemas con datos desbalanceados y está alineado con el objetivo del proyecto de optimizar el F1 Score sin sacrificar el desempeño general.

---

## Herramientas y Tecnologías
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Conclusión Clave
Este proyecto demuestra la aplicación de técnicas de machine learning para resolver un problema real de negocio, con enfoque en el desempeño del modelo y su interpretabilidad.



---



# Customer Churn Prediction – Beta Bank

## Problem
Customer churn is a critical issue in the banking sector, as losing clients directly impacts revenue.  
The goal of this project is to build a machine learning model capable of predicting whether a customer will leave the bank, enabling proactive retention strategies.

---

## Data
The dataset contains customer-related features such as:

- **Demographics:** age, geography, gender  
- **Account information:** balance, tenure, number of products  
- **Activity indicators:** credit card usage, active membership  

The data presented **class imbalance**, which required additional preprocessing techniques.

---

## Approach
The project followed a structured machine learning workflow:

- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model training and evaluation  

Several models were tested:

- Logistic Regression  
- Decision Tree  
- Random Forest  

To address class imbalance, both **upsampling** and **downsampling** techniques were applied.

---

## Results
The best-performing model was **Random Forest with upsampling**, achieving:

- **F1 Score:** 0.626  
- **ROC AUC:** 0.856  

### Other key results:
- Random Forest (baseline): F1 = 0.601, ROC AUC = 0.850  
- Downsampling models improved recall but reduced precision  
- Logistic Regression showed lower overall performance  
- Decision Trees performed moderately but were less stable than ensemble methods  

The ROC curve demonstrated strong classification capability, indicating a good balance between true positive and false positive rates.

---

## Conclusion
The **Random Forest model with upsampling** proved to be the most effective approach for predicting customer churn. It achieved the best balance between precision and recall, while maintaining strong discriminative power.

This model is a robust solution for churn prediction under imbalanced data conditions and aligns with the project goal of optimizing F1 Score without sacrificing overall performance.

---

## Tools and Technologies
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Key Takeaway
This project demonstrates the application of machine learning techniques to solve a real-world business problem, with a focus on model performance and interpretability.
