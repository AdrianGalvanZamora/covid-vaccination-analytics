# Análisis y Predicción de Datos de Vacunación

## Descripción del Proyecto
Este proyecto analiza el dataset COVID-19 Vaccination Progress de Our World in Data para explorar tasas de vacunación globales y predecir trends en enfermedades infecciosas. Es relevante para salud pública, biotech y planificación de pandemias.

- **Dataset:** COVID-19 Vaccination Progress (196246 instancias, 16 features).
- **Fuente:** https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/vaccinations/vaccinations.csv
- **Herramientas:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn), Tableau Public.
- **Objetivos:**
  - EDA para identificar patrones por lugar y tiempo.
  - Manejo de NaN (imputación con forward-fill y mediana).
  - Pruebas de hipótesis (e.g., asociación entre vacunación y lugar).
  - Modelado con Random Forest (RMSE ~20-30, R² ~0.6-0.8 ajustado).
  - Dashboard interactivo en Tableau.

## Requisitos
- Python 3.8+.
- Bibliotecas: `pip install pandas numpy matplotlib seaborn scikit-learn scipy`.
- Dataset: `vaccinations.csv` (descarga desde la fuente).
- Tableau Public[](https://public.tableau.com).

## Metodología
1. **Carga y Limpieza:** Dataset con 196246 filas, manejo de ~50-70% NaN.
2. **EDA:** Distribuciones (e.g., total_vaccinations_per_hundred ~124), correlaciones altas.
3. **Pruebas:** Chi-cuadrado (p-value 5.22e-44) confirma asociación.
4. **Modelado:** Random Forest, ajustado para evitar leakage.
5. **Visualizaciones:** Histogramas, boxplots, mapa de calor, dashboard Tableau.

## Resultados Clave
- **RMSE:** ~20-30 (ajustado).
- **R²:** ~0.6-0.8 (ajustado).
- **Predictor clave:** daily_vaccinations (ajustado).
- **Insights:** Variación por lugar, útil para campañas de vacunación.
- **Limitaciones:** Multicolinealidad y posible leakage inicial.

## Cómo Ejecutar
1. Descarga `vaccinations.csv` y colócalo en la carpeta.
2. Abre `Proyecto_vacunas.ipynb` en Jupyter Notebook.
3. Ejecuta las celdas en orden (tarda ~2 minutos).
4. Usa `vaccinations_clean.csv` en Tableau.

## Tableau Dashboard
- Mapa global de tasas de vacunación.
- Gráfico de líneas por lugar y fecha.
- Filtros interactivos. Enlace: [Inserta enlace tras publicar].

## Mejoras Futuras
- Incluir datos de casos COVID.
- Optimizar modelo con GridSearchCV.
- Agregar predicciones temporales.
