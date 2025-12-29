# 🚢 Titanic Survival Analysis & Machine Learning

Este proyecto consiste en un **análisis exploratorio de datos (EDA)** y la **preparación de un modelo de Machine Learning** para predecir la supervivencia de los pasajeros del Titanic, utilizando el dataset clásico de Kaggle.

El objetivo principal es **analizar los factores que influyeron en la supervivencia** y construir un pipeline de datos limpio y reproducible orientado a ML.

---

## 📊 Dataset

- Fuente: Kaggle – *Titanic: Machine Learning from Disaster*
- Observaciones: 891 pasajeros
- Variables principales:
  - `survived` (variable objetivo)
  - `sex`
  - `age`
  - `fare`
  - `pclass`
  - `sibsp`, `parch`
  - Otras variables categóricas y numéricas

---

## 🔍 Análisis Exploratorio (EDA)

Durante el análisis exploratorio se estudiaron:

- Distribución de supervivientes vs no supervivientes
- Relación entre:
  - Sexo y supervivencia
  - Edad y supervivencia
  - Tarifa (`fare`) y clase social
- Visualización de distribuciones mediante:
  - Histogramas
  - Gráficos segmentados por supervivencia y sexo

Ejemplo de hipótesis analizadas:
- ¿Sobrevivieron más mujeres que hombres?
- ¿Influye la edad en la probabilidad de supervivencia?
- ¿Existe una relación entre clase social, tarifa y supervivencia?

---

## 🧹 Limpieza y Preprocesamiento de Datos

### Tratamiento de valores nulos

Se detectaron valores faltantes principalmente en:

- `age`
- `fare`

Estrategia aplicada:

| Variable | Estrategia | Justificación |
|--------|-----------|--------------|
| `age`  | Media     | Distribución relativamente simétrica |
| `fare` | Mediana   | Distribución sesgada con outliers |

Se evitó el uso de operaciones `inplace` para garantizar compatibilidad con versiones modernas de `pandas`.

---

## 🤖 Preparación para Machine Learning

El dataset se prepara para su uso en modelos de ML siguiendo buenas prácticas:

- Copia del DataFrame original
- Imputación de valores nulos sin *data leakage*
- Análisis de variables relevantes
- Base preparada para:
  - Codificación de variables categóricas
  - Escalado
  - Modelos supervisados (Logistic Regression, Random Forest, etc.)

---

## 🧠 Conclusiones del Análisis

Algunas conclusiones preliminares:

- El sexo es una de las variables más determinantes en la supervivencia
- La edad influye, especialmente en niños y adultos jóvenes
- La tarifa y la clase social muestran una fuerte relación con la probabilidad de supervivencia

Estas observaciones justifican su inclusión como *features* clave en el modelo predictivo.

---

## 🛠️ Tecnologías Utilizadas

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn (preparado para uso posterior)

---

## 🚀 Próximos Pasos

- Codificación de variables categóricas
- Creación de pipelines con `sklearn`
- Entrenamiento de modelos
- Evaluación y comparación de métricas
- Optimización de hiperparámetros

---

## 👤 Autor

Proyecto realizado por **Raúl Revidiego**  
Enfoque en aprendizaje, buenas prácticas y reproducibilidad en Ciencia de Datos.

---

## 📌 Nota

Este proyecto tiene fines educativos y forma parte del aprendizaje práctico en **Data Science y Machine Learning**.


