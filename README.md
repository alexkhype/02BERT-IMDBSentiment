# Análisis de Sentimiendo en Reseñas de IMDB

## Tabla de Contenidos
- [Descripción](#Descripción)
- [Datos](#Datos)
- [Análisis](#Análisis)
- [Tecnologías y herramientas](#Tecnologías-y-herramientas)
- [Resultados](#Resultados)
- [Contribuciones](#Contribuciones)
- [Licencia](#Licencia)
- [Contacto](#Contacto)

## Descripción
Este proyecto utiliza modelos de aprendizaje automático para clasificar reseñas positivas y negativas de películas, entrenados con un conjunto de datos IMDB que contiene más de 47,000 reseñas. El objetivo es automatizar la detección de críticas para Film Junky Union, evaluando el rendimiento con la métrica F1.

## Datos
Se utilizó un conjunto de datos principal:  
- **games.csv**: DataFrame con 47,331 registros y 17 columnas que incluyen metadatos de películas (titulos, géneros, años), puntuaciones, reseñas y variables numéricas y categóricas, con datos mayormente completos y tipos variados.

## Análisis
El enfoque incluyó:  
- Uso de Python con librerías NLP (NLTK, spaCy), machine learning (scikit-learn, LightGBM) y visualización (matplotlib, seaborn).
- Limpieza y normalización de datos, imputación y eliminación de valores faltantes, y selección de variables relevantes.
- Análisis exploratorio (EDA) para entender distribución y balance de reseñas positivas/negativas, y tendencias temporales.
- Implementación de función de preprocesamiento con lematización y eliminación de stopwords; división clara entre conjuntos de entrenamiento y prueba.
- Entrenamiento y comparación de múltiples modelos: DummyClassifier, regresión logística, Random Forest, LightGBM y BERT embeddings (limitados).

## Tecnologías y herramientas
- Python 3.9 para desarrollo general y scripting.
- Pandas, NumPy para manipulación y análisis de datos.
- Matplotlib, Seaborn para creación de visualizaciones y análisis gráfico.
- NLTK y spaCy para procesamiento de lenguaje natural y lematización.
- Scikit-learn y LightGBM para construcción y evaluación de modelos de aprendizaje automático.
- Transformers y PyTorch para experimentación con modelos de lenguaje profundo (BERT).
- Jupyter Notebook para desarrollo interactivo y presentación de análisis.

## Resultados
- Regresión logística con NLTK/spaCy y TF-IDF alcanzó F1 de 0.88, siendo rápido y eficiente.
- LightGBM obtuvo F1 de 0.85 pero con tiempos de predicción más largos.
- Random Forest alcanzó F1 de 0.83, por debajo del umbral deseado.
- Modelos con BERT mostraron sobreajuste y bajo desempeño (F1 < 0.65).
- Regresión logística demostró robustez incluso en reseñas breves; recomendada para producción.

## Contribuciones
Bienvenidas sugerencias, correcciones y nuevas visualizaciones. Por favor, abre un issue o pull request para colaborar.

## Licencia
Este proyecto está bajo la licencia MIT.

## Contacto
Nombre: Alejandro M. García  
Email: [alexkhype@gmail.com](mailto:alexkhype@gmail.com)  
LinkedIn: [linkedin.com/in/amggl](https://linkedin.com/in/amggl)
