# SUPPORT2 - Predicción de Supervivencia en Pacientes Críticos

## Autores
- Miguel Angel Puerta Vasquez - ID: 1000760164
- Leon Mateo Velez Gonzáles - ID: 1216728793
- Universidad de Antioquia - Modelos y Simulación II
- Profesor: Julian David Arias Londono

## Recursos del Proyecto

### Documento del Proyecto (Proyecto_Modelos_II_Documento.pdf)
Contiene toda la metodología, análisis detallado y resultados completos del proyecto.

### Código en Google Colab
Enlace: https://colab.research.google.com/drive/1Zs2acsEpPw8v8xSYtCybNXCcz86Zrg_u#scrollTo=v5LGHAkvFHfs
Ejecuta todo el código directamente en tu navegador sin necesidad de instalaciones locales.

### Video Explicativo
Enlace: https://youtube.com/
Video de 10 minutos con explicación completa del proyecto y demostración práctica.

---

## Guía de Reproducción de Resultados

### Acceso al Notebook de Google Colab

1. Abrir el Notebook
   - Haz clic en el enlace de Google Colab proporcionado arriba
   - Se abrirá el notebook en tu navegador web
  
2. Cargar Archivo con DataSet
   - Descargar dataSet del repositorio
   - Dar click en archivos dentro de Google Colab
   - Cargar alchivo al almacenamiento de la sesion

3. Ejecutar el Código
     - Ejecutar paso a paso
     - Ve celda por celda
     - Presiona Ctrl + Enter para ejecutar cada celda
     - Sigue el orden secuencial del notebook

### Contenido del Notebook Colab

El notebook está organizado en las siguientes secciones:

#### 1. Instalación e Importación de Librerías
- Instalación de todas las dependencias necesarias
- Importación de bibliotecas de machine learning
- Configuración de visualizaciones

#### 2. Carga y Exploración del Dataset
- Descarga automática del dataset SUPPORT2
- Análisis exploratorio inicial de los datos
- Visualización de la distribución de variables
- Identificación de valores faltantes

#### 3. Preprocesamiento de Datos
- Imputación de valores faltantes según la metodología del proyecto
- Codificación de variables categóricas
- Escalado de variables numéricas
- División en conjuntos de entrenamiento, validación y prueba

#### 4. Entrenamiento de Modelos

Se entrenan y optimizan 5 modelos diferentes:

**Modelo 1: Regresión Lineal**
- Ajuste de hiperparámetros con Grid Search
- Validación cruzada estratificada

**Modelo 2: K-Vecinos Más Cercanos (KNN)**
- Optimización de número de vecinos
- Prueba de diferentes métricas de distancia

**Modelo 3: Random Forest**
- Optimización de número de estimadores
- Ajuste de profundidad máxima y muestras por división

**Modelo 4: Red Neuronal (MLP)**
- Optimización de capas ocultas
- Prueba de funciones de activación
- Ajuste de tasa de aprendizaje

**Modelo 5: Máquinas de Soporte Vectorial (SVM)**
- Optimización del parámetro C
- Prueba de diferentes kernels

#### 5. Evaluación y Comparación de Modelos
- Cálculo de métricas de desempeño (MAE, RMSE, R²)
- Comparación visual del rendimiento
- Selección del mejor modelo
- Análisis de importancia de variables

#### 6. Reducción de Dimensionalidad
- Aplicación de PCA para reducción de características
- Prueba con UMAP para visualización
- Evaluación del impacto en el rendimiento

#### 7. Resultados Finales
- Tablas comparativas de métricas
- Gráficas de desempeño por modelo
- Heatmap de correlaciones
- Análisis de variables más importantes

### Resultados Esperados

Al ejecutar completamente el notebook, deberías obtener:

1. Métricas de los Modelos
   - Random Forest: MAE ~0.026, RMSE ~0.043, R² ~0.970
   - Regresión Lineal: MAE ~0.051, RMSE ~0.075, R² ~0.910
   - Comparativa completa de los 5 modelos

2. Visualizaciones Generadas
   - Gráfica de comparación de modelos
   - Heatmap de correlaciones entre variables
   - Importancia de características del Random Forest
   - Resultados de reducción dimensional

3. Análisis de Variables
   - Identificación de las variables más relevantes
   - Impacto de cada variable en la predicción
   - Correlaciones entre variables objetivo
