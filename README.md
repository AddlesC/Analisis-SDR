# Análisis de Señales de Voltaje 

Este repositorio contiene scripts de Python para la carga, corrección de offset, filtrado por amplitud, y visualización de señales de voltaje. Se utiliza Matplotlib para la visualización de los datos, opcionalmente se usa Plotly para la visualizacion interactiva.

## Descripción

El proyecto se enfoca en procesar y analizar señales de voltaje, específicamente en:

- Corrección de offset basada en un rango de baseline predefinido.
- Filtrado de pulsos por amplitud negativa y visualización de los seleccionados.
- Generación de histogramas para visualizar la distribución de las amplitudes corregidas que superan un umbral negativo.

## Proceso

### 1. Corrección de Offset en Señales de Voltaje

Calcula un segmento de la señal para determinar el offset y lo resta de toda la señal para corregirla. Las señales ajustadas se visualizan luego utilizando Plotly.

### 2. Filtrado de Pulsos por Amplitud

Filtra los pulsos corregidos por offset, seleccionando solo aquellos que superan un umbral negativo específico dentro de un intervalo de tiempo predefinido. Los resultados se visualizan mostrando los pulsos que cumplen con estos criterios.

### 3. Histograma de Amplitudes Corregidas

Construye un histograma de las amplitudes corregidas que exceden un umbral negativo, recopilando estas amplitudes de los pulsos seleccionados y visualizando la distribución de sus valores.

### 4. Guardado en ROOT

Se transcriben los datos del histograma a formato root, herramienta que permite una visualizacion interactiva, pudiendo calcular y modificar diferentes parametros.

## Análisis Interactivo de Señales de Voltaje

Para una exploración detallada y un análisis interactivo de las señales de voltaje, proporcionamos una visualización completa utilizando Plotly.

Acceda al análisis interactivo a través del siguiente enlace: [Visualización Interactiva de Señales de Voltaje](https://drive.google.com/file/d/1yYJdzBc_tnzKvMe-skEK3YgvXNz5kuAX/view?usp=sharing).

## Herramientas Utilizadas

- **Pandas** para la manipulación y análisis de los datos.
- **NumPy** para el cálculo de operaciones matemáticas.
- **Matplotlib** para la generacion de graficos
- **Plotly** para la generación de gráficos interactivos.
- **Uproot** para la conversion a formato ROOT

## Cómo Usar

1. Asegúrese de tener todas las dependencias instaladas.
2. Ejecute los scripts en un entorno Jupyter para una experiencia interactiva.
3. Ajuste los umbrales y rangos según los requisitos de su análisis.


