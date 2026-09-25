# Laboratorio Práctico: Predicción de Costos de Envío (Logística E-Commerce)

Desarrollo de un modelo predictivo de Machine Learning orientado a estimar los costos de despacho para paquetes, abarcando desde la limpieza de datos y codificación de variables hasta el entrenamiento y validación de un algoritmo de regresión lineal.

## Integrantes - Grupo 07 

* **Javiera Cuevas** – [javiera.cuevas2201@alumnos.ubiobio.cl](mailto:javiera.cuevas2201@alumnos.ubiobio.cl)
* **Antonia Peña** – [antonia.pena2202@alumnos.ubiobio.cl](mailto:antonia.pena2202@alumnos.ubiobio.cl)
* **Arline Mitchell** – [arline.mitchell2201@alumnos.ubiobio.cl](mailto:arline.mitchell2201@alumnos.ubiobio.cl)
* **Nicolás Morales** – [nicolas.morales2001@alumnos.ubiobio.cl](mailto:nicolas.morales2001@alumnos.ubiobio.cl)

## Contexto del Problema y Descripción

* Una empresa de logística de e-commerce necesita estimar el Costo Total de Envío (`costo_envio`) en USD para cada paquete antes de procesarlo. 
* El objetivo principal del desarrollo de este modelo es lograr ajustar las tarifas de cobro en tiempo real dentro de su sitio web.

## Contenidos del Notebook

El desarrollo de este laboratorio sigue las instrucciones prácticas exigidas y está estructurado en las siguientes fases:

1. **Paso 1 - Limpieza Express:** 
   * Carga del conjunto de datos mediante el archivo `lab_costos_envio.csv`.
   * Tratamiento rápido de nulos, efectuando la imputación de los valores faltantes en las variables `peso_kg` y `distancia_km` utilizando la medida estadística que resulte más conveniente para cada columna.
2. **Paso 2 - Codificación de Variables:**
   * Preparación y codificación de las variables predictoras para poder ingresarlas al modelo de aprendizaje.
3. **Paso 3 - Entrenamiento (Train/Test Split y Modelo):**
   * División de los datos para lograr entrenar y posteriormente probar el modelo.
   * Entrenamiento de un modelo de Regresión Lineal utilizando la librería `Linear Regression` de scikit-learn.
4. **Paso 4 - Evaluación de Restricciones:**
   * Cálculo de las métricas de validación del modelo, específicamente el $R^{2}$ y MAE.
   * Verificación para comprobar si el modelo elaborado cumple con las Restricciones Mínimas de Aprobación.

## Umbrales de Evaluación

El modelo de Regresión Lineal fue ajustado y evaluado para cumplir estrictamente con los siguientes requisitos:

* **Métrica $R^{2}$:** El umbral mínimo requerido para aprobar es de un $R^{2} > 0.90$. El resultado esperado como solución ideal se encuentra aproximadamente entre 0.96 y 0.97
* **Métrica MAE:** El umbral mínimo exigido es mantener el error MAE <= 3.50 USD. El resultado ideal proyectado debería oscilar aproximadamente entre 2.70 y 2.85 USD

## Estructura del Repositorio

```text
├── Lab_Regresion/
│   ├── Lab_Costos_Envio.ipynb               # Notebook principal con la limpieza, entrenamiento y métricas
│   └── lab_costos_envio.csv                 # Dataset original proporcionado para el problema
└── README.md                                # Documentación del repositorio
