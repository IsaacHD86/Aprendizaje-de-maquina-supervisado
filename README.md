# Aprendizaje-de-maquina-supervisado
Regresion lineal simple.

# Análisis de Regresión para Pronóstico del PIB de México

Este proyecto tiene como objetivo construir un **modelo predictivo** utilizando análisis de regresión lineal aplicado a los datos históricos del **Producto Interno Bruto (GDP)** de México. Los datos provienen de la base de datos del Banco Mundial y se encuentran en el archivo Excel titulado **“Mexico GDP.xlsx”**.

## Descripción del Proyecto

El análisis se centra en ajustar un **modelo logístico** mediante regresión de mínimos cuadrados, con el fin de predecir el crecimiento económico de México en función del tiempo (años). A partir de los datos disponibles, se realizará una **normalización** y un ajuste de los datos para obtener predicciones precisas.

### Objetivos:

1. **Análisis Exploratorio de los Datos**:
   - Importar y analizar los datos históricos del PIB de México.
   - Visualizar la tendencia del PIB a lo largo de los años mediante gráficos.

2. **Ajuste de Modelo Logístico**:
   - Implementar una regresión de mínimos cuadrados para ajustar los datos históricos a un **modelo logístico**.
   - Estimar los parámetros **Beta1** y **Beta2** del modelo.
   - Evaluar si hubo problemas en la estimación de parámetros y analizar sus posibles causas.

3. **Normalización de Datos**:
   - Transformar los datos históricos mediante **normalización**, dividiendo cada observación por el valor máximo de su columna correspondiente.
   - Volver a ajustar el modelo con los datos normalizados para observar posibles mejoras en la precisión de las predicciones.

## Metodología

### 1. Preparación de Datos

- Descargar y abrir el archivo **“Mexico GDP.xlsx”**.
- Importar los datos utilizando **Pandas** y realizar un análisis exploratorio inicial:
  - Visualizar las primeras filas del dataset.
  - Comprobar la existencia de valores nulos y tratar datos faltantes si es necesario.
- Graficar la evolución del **PIB** a lo largo del tiempo utilizando **Matplotlib**.

### 2. Ajuste del Modelo Logístico

El modelo logístico a utilizar es de la forma:
\[
Y = \frac{1}{1 + e^{-(\beta_1 + \beta_2 X)}}
\]
donde:
- **X** es el período (año).
- **Y** es el PIB normalizado.
- **Beta1** y **Beta2** son los parámetros a estimar.

**Pasos para el ajuste**:
- Utilizar **SciPy** para realizar la regresión de mínimos cuadrados.
- Evaluar el **Error Cuadrático Medio (MSE)** y el **Coeficiente de Determinación (R²)** para validar el modelo.
- Analizar posibles problemas en la convergencia del modelo o estimación de parámetros.

### 3. Normalización de los Datos

- Para mejorar la precisión y estabilidad del modelo, se normalizan los datos dividiendo cada observación por el valor máximo de su columna.
- Ajustar nuevamente el modelo utilizando los datos normalizados.
- Comparar el desempeño entre el modelo con datos originales y el modelo con datos normalizados.

## Resultados y Análisis

- **Parámetros del Modelo**: Documentar los valores obtenidos para **Beta1** y **Beta2**.
- **Precisión del Modelo**: Evaluar el rendimiento utilizando métricas como **MSE** y **R²**.
- **Discusión de Problemas**:
  - Analizar posibles dificultades en la estimación de parámetros, como **sobreajuste** o **falta de convergencia**.
  - Identificar si la normalización mejoró la precisión del modelo.

## Requisitos del Proyecto

Para ejecutar el análisis, asegúrate de tener instaladas las siguientes bibliotecas:

- **Pandas**: Para la manipulación y análisis de datos.
- **NumPy**: Para cálculos matemáticos avanzados.
- **SciPy**: Para la implementación de la regresión de mínimos cuadrados.
- **Matplotlib/Seaborn**: Para la visualización de gráficos.
  
## Autor
Isaac Heredia Diaz
[GitHub](https://github.com/IsaacHD86)

