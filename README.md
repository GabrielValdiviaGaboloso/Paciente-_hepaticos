# Proyecto: Análisis y Clasificación de Pacientes Hepáticos

## Introducción y Objetivos

Este proyecto tiene como objetivo analizar y construir modelos de clasificación para predecir si un paciente tiene una condición hepática (`is_patient`). Se busca entender las relaciones entre las variables clínicas y evaluar la capacidad predictiva de distintos modelos de machine learning. El propósito final es identificar patrones útiles para apoyar diagnósticos tempranos en un entorno clínico.

## Descripción del Conjunto de Datos

El dataset contiene información de pacientes con distintas variables clínicas como edad, género, niveles de bilirrubina total y directa, enzimas hepáticas (SGPT, SGOT), proteínas totales, albúmina, fosfatasa alcalina, y la relación albúmina/globulina. La variable objetivo `is_patient` indica si el paciente tiene la condición hepática (1 = Sí, 0 = No).

## Principales Análisis y Hallazgos

- Análisis exploratorio para comprender la distribución y correlaciones entre variables.
- Baja correlación directa entre la mayoría de las variables independientes y la variable objetivo.
- Desbalance en las clases del dataset (más pacientes positivos que negativos).
- Evaluación de varios modelos de machine learning para la predicción.

## Visualizaciones Clave

- **Mapa de calor de correlación:** muestra las relaciones entre variables, sin correlaciones fuertes que expliquen el target.
- **Curvas ROC:** comparación de capacidad discriminativa de modelos, con un AUC máximo cercano a 0.74.
- **Boxplots:** comparación de variables clave entre pacientes sanos y enfermos.

## Conclusiones y Recomendaciones

Los modelos alcanzaron un rendimiento moderado (accuracy y AUC < 0.7), probablemente debido a la limitada información predictiva y al desbalance de clases. Se recomienda:

- Recolectar más datos y variables clínicas relevantes.
- Aplicar técnicas para manejar desbalance en las clases.
- Incorporar biomarcadores o datos adicionales.
- Validar modelos en datos externos para asegurar robustez clínica.
