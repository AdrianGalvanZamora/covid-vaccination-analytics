# 🧬 Análisis y Predicción Global de Vacunación contra COVID-19  
[English version below ⬇️]  

**Sector:** Salud pública, Biotech, Planificación sanitaria  
**Herramientas:** Python (Pandas, NumPy, Seaborn, Scikit-learn), Tableau Public  

---

## 📋 Descripción General  
Este proyecto explora los datos de vacunación global contra COVID-19 recopilados por *Our World in Data* con dos objetivos principales:  
1. **Analizar las tendencias de vacunación a nivel mundial** para identificar disparidades geográficas y temporales.  
2. **Predecir la evolución de la cobertura vacunal** mediante un modelo de *Random Forest*, con potencial aplicación en campañas de salud pública y estrategias de distribución.  

El análisis combina técnicas de exploración de datos (EDA), pruebas estadísticas y visualizaciones interactivas en Tableau para ofrecer una visión integral del progreso y los factores asociados a la vacunación.

---

## 📊 Dataset  
- **Fuente:** [Our World in Data – COVID-19 Vaccination Progress](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/vaccinations/vaccinations.csv)  
- **Tamaño:** 196 246 registros, 16 variables  
- **Cobertura:** Países y regiones a nivel global  

---

## 🔍 Metodología  
1. **Limpieza y Preparación de Datos**  
   - Manejo de valores faltantes (50–70 % NaN) mediante imputación forward-fill y mediana.  
   - Estandarización de variables y revisión de multicolinealidad.  

2. **Análisis Exploratorio (EDA)**  
   - Distribuciones y correlaciones entre indicadores de vacunación.  
   - Identificación de patrones temporales y geográficos.  
   - Prueba Chi-cuadrado (p = 5.22 × 10⁻⁴⁴) que confirma relación significativa entre tasa de vacunación y ubicación geográfica.  

3. **Modelado Predictivo**  
   - Algoritmo: *Random Forest Regressor*.  
   - Métricas de rendimiento: RMSE ≈ 20–30, R² ≈ 0.6–0.8.  
   - Variables más influyentes: `daily_vaccinations`, `people_fully_vaccinated_per_hundred`.  

4. **Visualización Interactiva**  
   - **Dashboard en Tableau:** mapa global, líneas de progreso por país y filtros dinámicos para comparación de regiones.  

---

## 🌎 Principales Hallazgos  
- Se detectaron **brechas sustanciales** en la cobertura de vacunación entre regiones.  
- El ritmo diario de vacunación es el **predictor más fuerte** del avance general.  
- La información es aplicable a **campañas de inmunización y planificación logística** de recursos sanitarios.  

---

## 🧠 Aplicación en el Mundo Real  
Este modelo puede ayudar a organismos de salud o startups de biotech a:  
- Priorizar regiones con baja cobertura vacunal.  
- Predecir cuellos de botella en la distribución.  
- Evaluar el impacto de políticas públicas y optimizar campañas de vacunación.  

---

## ⚙️ Requisitos de Ejecución  
- Python 3.8+  
- Librerías: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`  
- Archivo: `vaccinations.csv` (descargar desde la fuente)  
- Tableau Public (para visualizar el dashboard interactivo)  

---

## 🚀 Ejecución del Proyecto  
1. Clona este repositorio y coloca el dataset en la carpeta raíz.  
2. Abre `Proyecto_vacunas.ipynb` en Jupyter Notebook.  
3. Ejecuta todas las celdas (tiempo estimado: ~2 min).  
4. Exporta `vaccinations_clean.csv` y conéctalo a Tableau.  
5. Accede al dashboard interactivo: [**enlace a publicar**].  

---

## 📈 Resultados y Limitaciones  
- **Modelo satisfactorio**, aunque sensible a multicolinealidad inicial.  
- Posible mejora con *GridSearchCV* y *feature engineering* temporal.  
- Los resultados son indicativos; no sustituyen análisis epidemiológico formal.  

---

## 🔮 Mejoras Futuras  
- Integrar datos de casos confirmados y tasas de mortalidad.  
- Extender el modelo a series temporales (*ARIMA*, *Prophet*).  
- Automatizar actualización de datos mediante API.  

---

## 💡 Resumen Ejecutivo  
> Este proyecto demuestra la capacidad de transformar datos masivos en decisiones accionables para la salud pública. Utilizando Python para análisis predictivo y Tableau para visualización, el estudio ofrece una guía práctica para optimizar campañas de vacunación y prever la evolución de enfermedades infecciosas.  

---

## 🖼️ Recomendaciones Visuales  
- Incluye **una captura del dashboard de Tableau** (mapa global con gradiente de color y gráfico temporal).  
- Añade un gráfico de barras con las 5 variables más importantes del modelo (*feature importance*).  
- Publica el dashboard en **Tableau Public** y agrega el enlace con una miniatura.  

---

# 🇬🇧 COVID-19 Global Vaccination Analysis and Prediction  

**Industry:** Public Health, Biotech, Pandemic Planning  
**Tools:** Python (Pandas, NumPy, Seaborn, Scikit-learn), Tableau Public  

---

## 📋 Project Overview  
This project analyzes the global COVID-19 vaccination dataset from *Our World in Data* with two main goals:  
1. **Explore worldwide vaccination trends** to identify regional and temporal disparities.  
2. **Predict vaccination coverage progress** using a *Random Forest* model, supporting public health and distribution strategies.  

The analysis combines exploratory data analysis (EDA), statistical testing, and interactive Tableau dashboards to deliver actionable insights into global vaccination progress.  

---

## 📊 Dataset  
- **Source:** [Our World in Data – COVID-19 Vaccination Progress](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/vaccinations/vaccinations.csv)  
- **Size:** 196,246 records, 16 variables  
- **Scope:** Global coverage by country and region  

---

## 🔍 Methodology  
1. **Data Cleaning and Preparation**  
   - Handled 50–70% missing values with forward-fill and median imputation.  
   - Standardized features and reviewed multicollinearity.  

2. **Exploratory Data Analysis (EDA)**  
   - Analyzed variable distributions and correlations.  
   - Identified temporal and regional trends.  
   - Chi-square test (p = 5.22 × 10⁻⁴⁴) confirmed significant association between vaccination rate and geography.  

3. **Predictive Modeling**  
   - Algorithm: *Random Forest Regressor*  
   - Performance: RMSE ≈ 20–30, R² ≈ 0.6–0.8  
   - Key features: `daily_vaccinations`, `people_fully_vaccinated_per_hundred`  

4. **Interactive Visualization**  
   - **Tableau Dashboard:** global vaccination map, country-level progress lines, and dynamic filters for comparison.  

---

## 🌎 Key Findings  
- Large disparities in vaccination coverage across regions.  
- Daily vaccination rate is the **strongest predictor** of global progress.  
- Insights can guide **public health campaigns and resource allocation.**  

---

## 🧠 Real-World Application  
This model can help health organizations or biotech startups to:  
- Prioritize low-coverage regions.  
- Predict distribution bottlenecks.  
- Assess public health policy effectiveness and improve vaccination campaigns.  

---

## ⚙️ Setup Requirements  
- Python 3.8+  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`  
- Dataset: `vaccinations.csv` (download from source)  
- Tableau Public for visualization  

---

## 🚀 How to Run  
1. Clone the repository and place the dataset in the root folder.  
2. Open `Proyecto_vacunas.ipynb` in Jupyter Notebook.  
3. Run all cells (runtime ≈ 2 minutes).  
4. Export `vaccinations_clean.csv` and connect it to Tableau.  
5. Access the interactive dashboard: [**to be published**].  

---

## 📈 Results and Limitations  
- Satisfactory model performance with moderate multicollinearity.  
- Further tuning with *GridSearchCV* and temporal feature engineering recommended.  
- Results are indicative and not a substitute for epidemiological modeling.  

---

## 🔮 Future Improvements  
- Integrate case and mortality data.  
- Extend to time series models (*ARIMA*, *Prophet*).  
- Automate updates via API.  

---

## 💡 Executive Summary  
> This project demonstrates how to transform large-scale public health data into actionable insights. Using Python for predictive modeling and Tableau for visualization, it provides a practical framework to support vaccination strategies and infectious disease forecasting.  

---

## 🖼️ Visual Recommendations  
- Include a screenshot of the Tableau dashboard (global map + time series).  
- Add a feature importance plot from the Random Forest model.  
- Publish the Tableau dashboard and embed the link or thumbnail.  
