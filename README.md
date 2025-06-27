#  Stress Level Prediction using Machine Learning

##  Problem Statement

This project aims to **predict individuals' stress levels** based on behavioral, physiological, and lifestyle-related variables. Understanding and anticipating stress levels can support early interventions and promote healthier daily habits, improving both mental and physical well-being.

##  Dataset

The dataset used in this project is the publicly available **Sleep and Mental Health Dataset**, which can be found on the profile of Laksika Tharmalingam on [Kaggle]([https://www.kaggle.com/datasets/sujaykapadnis/sleep-and-mental-health-dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)).

### Dataset Overview:

- **Total instances**: 370
- **Target variable**: `Stress Level` (continuous)
- **Features include**:
  - Sleep Duration
  - Quality of Sleep (1–10)
  - Physical Activity Level
  - BMI and BMI Category
  - Occupation
  - Sleep Disorder
  - Age, Gender, and more

The dataset includes both **numerical and categorical features**, and it reflects a mix of healthy and stressed individuals from different professional backgrounds.

##  Solution Approach

The solution follows a complete supervised learning workflow:

1. **Exploratory Data Analysis (EDA)**:
   - Distribution plots and outlier detection
   - Correlation analysis (Spearman)
   - Kruskal-Wallis test for group comparisons

2. **Preprocessing**:
   - Handling missing values
   - Encoding categorical variables
   - Feature scaling (when required)

3. **Model Training and Evaluation**:
   - Several regression models were tested, including Linear Regression and Ridge Regression.
   - A **Random Forest Regressor** was selected as the most robust model after:
     - GridSearchCV hyperparameter tuning
     - 5-fold cross-validation
   - Final model achieved:
     - **R² on test set**: 0.9731
     - **MAE on test**: 0.1171

4. **Interpretation & Insights**:
   - Features such as **Sleep Duration**, **Physical Activity**, and **Sleep Quality** showed strong negative correlations with stress.
   - Occupation and Sleep Disorder were statistically significant according to the Kruskal-Wallis test.
   - These findings provide **not only predictive value but also actionable lifestyle insights**.

##  Repository Contents

- `notebooks/`: Jupyter notebooks with EDA, modeling, and evaluation.
- `models/`: Saved models (e.g., Random Forest).
- `figures/`: Plots and graphs used in the analysis.
- `README.md`: Project overview and documentation.


##  License

This project is for educational purposes and uses a public dataset. All of the conclusions are made with an **educational perspective**. I am not a proffesional of this sector.

---

#  Predicción del Nivel de Estrés con Machine Learning

##  Descripción del Problema

Este proyecto tiene como objetivo **predecir el nivel de estrés de las personas** a partir de variables conductuales, fisiológicas y relacionadas con el estilo de vida. Comprender y anticipar los niveles de estrés puede favorecer intervenciones tempranas y fomentar hábitos diarios más saludables, mejorando tanto el bienestar mental como físico.

##  Dataset

El dataset utilizado en este proyecto es público y se encuentra disponible como **Sleep and Mental Health Dataset** en el perfil de Laksika Tharmalingam en [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset).

### Descripción general del dataset:

- **Número total de registros**: 370  
- **Variable objetivo**: `Stress Level` (continua)  
- **Variables incluidas**:
  - Duración del sueño  
  - Calidad del sueño (escala 1–10)  
  - Nivel de actividad física  
  - IMC y categoría de IMC  
  - Ocupación  
  - Trastorno del sueño  
  - Edad, género, entre otras  

El dataset contiene tanto **variables numéricas como categóricas** y representa una mezcla de individuos sanos y con estrés de diversas profesiones.

## 🛠 Enfoque de la Solución

La solución adoptada sigue un flujo completo de aprendizaje supervisado:

1. **Análisis Exploratorio de Datos (EDA)**:
   - Gráficas de distribución y detección de outliers  
   - Análisis de correlación (Spearman)  
   - Test de Kruskal-Wallis para comparación de grupos

2. **Preprocesamiento**:
   - Tratamiento de valores faltantes  
   - Codificación de variables categóricas  
   - Escalado de características (cuando es necesario)

3. **Entrenamiento y Evaluación del Modelo**:
   - Se probaron varios modelos de regresión, incluyendo Regresión Lineal y Ridge.  
   - Se seleccionó un **Random Forest Regressor** como modelo más robusto tras:
     - Ajuste de hiperparámetros con GridSearchCV  
     - Validación cruzada con 5 folds  
   - Rendimiento del modelo final:
     - **R² en test**: 0.9731  
     - **MAE en test**: 0.1171  

4. **Interpretación y Conclusiones**:
   - Variables como **Duración del Sueño**, **Actividad Física** y **Calidad del Sueño** mostraron fuertes correlaciones negativas con el estrés.  
   - Las variables **Ocupación** y **Trastorno del Sueño** resultaron estadísticamente significativas según el test de Kruskal-Wallis.  
   - Estos hallazgos aportan **valor predictivo y recomendaciones aplicables al estilo de vida**.

##  Contenido del Repositorio

- `notebooks/`: Notebooks de Jupyter con el EDA, modelado y evaluación.  
- `models/`: Modelos guardados (por ejemplo, Random Forest).  
- `figures/`: Gráficas y visualizaciones utilizadas en el análisis.  
- `README.md`: Documentación general del proyecto.

##  Licencia

Este proyecto tiene fines educativos y utiliza un dataset público. Todas las conclusiones están hechas desde una **perspectiva académica y de aprendizaje**. No soy profesional de la salud ni de la psicología.

