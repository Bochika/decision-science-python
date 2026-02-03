# Análisis de la dinámica histórica de la Laguna de Fúquene usando Observación de la Tierra (EO)

## 1. Contexto del problema

La Laguna de Fúquene es uno de los cuerpos de agua continentales más importantes del altiplano cundiboyacense en Colombia. Su extensión, dinámica hidrológica y estado ecológico han cambiado de manera significativa en las últimas décadas debido a factores naturales y antrópicos, como la variabilidad climática, la regulación hidráulica y el uso del suelo.

El monitoreo continuo de este tipo de ecosistemas es complejo debido a la limitada disponibilidad de datos in situ consistentes a largo plazo. En este contexto, la Observación de la Tierra (Earth Observation, EO) ofrece una alternativa robusta para analizar cambios espaciales y temporales mediante imágenes satelitales históricas.

---

## 2. Pregunta de investigación

**¿Cómo ha cambiado espacial y temporalmente el espejo de agua de la Laguna de Fúquene entre 1985 y 2024 utilizando datos de Observación de la Tierra?**

El objetivo del proyecto no es estimar el área exacta del espejo de agua, sino identificar **tendencias, patrones espaciales y variabilidad temporal** a partir de una metodología consistente.

---

## 3. Datos utilizados

### 3.1 Observación de la Tierra (EO)

En este proyecto se emplean datos de Observación de la Tierra (EO), entendidos como información obtenida mediante sensores remotos que capturan características físicas de la superficie terrestre desde plataformas satelitales.

### 3.2 Satélites

Se utilizaron imágenes de la misión **Landsat**, debido a su cobertura temporal extensa y consistente:

* Landsat 5 TM
* Landsat 7 ETM+
* Landsat 8 OLI
* Landsat 9 OLI-2

**Resolución espacial:** 30 m
**Periodo de análisis:** 1985–2024
**Plataforma:** Google Earth Engine (GEE)

Aunque sensores más recientes como Sentinel-2 ofrecen mayor resolución espacial, no fueron utilizados para el análisis histórico debido a su cobertura temporal limitada (post-2015).

---

## 4. Metodología

### 4.1 Delimitación espacial

Se definió un polígono de interés (ROI) fijo que representa el entorno de la laguna. Este polígono fue validado visualmente y se mantuvo constante durante todo el periodo de análisis para evitar sesgos derivados de cambios en la geometría.

### 4.2 Detección del cuerpo de agua

Para identificar el espejo de agua se utilizó el **Índice de Diferencia Normalizada de Agua (NDWI)**, calculado a partir de las bandas verde e infrarrojo cercano de Landsat.

Se aplicó un umbral constante para clasificar los píxeles como agua/no agua, priorizando la consistencia metodológica sobre la optimización puntual del índice.

### 4.3 Resolución temporal y decisiones metodológicas

Inicialmente se exploró un análisis mensual y anual del área de la laguna. Sin embargo, el análisis mensual presentó múltiples limitaciones:

* Alta nubosidad en ciertos periodos
* Ausencia de imágenes válidas en algunos meses
* Resultados inconsistentes y numerosos valores faltantes

Como resultado, se tomó la decisión de:

* Utilizar **series temporales anuales** para analizar tendencias generales
* Generar **mapas espaciales cada 5 años** para evaluar visualmente los cambios en la extensión del espejo de agua

Esta decisión permitió balancear detalle temporal, calidad de datos y confiabilidad de los resultados.

---

## 5. Resultados

Los principales hallazgos del análisis incluyen:

* Presencia de una alta variabilidad interanual en la extensión del espejo de agua
* Cambios espaciales evidentes en los bordes de la laguna al comparar mapas quinquenales
* Diferencias entre los valores derivados de EO y cifras reportadas oficialmente, atribuibles a diferencias metodológicas y de resolución

Los mapas generados cada 5 años permiten observar patrones espaciales consistentes que complementan el análisis temporal.

---

## 6. Discusión y limitaciones

Este estudio presenta varias limitaciones importantes:

* La resolución espacial de 30 m limita la detección de cambios pequeños en el borde del cuerpo de agua
* La nubosidad afecta la disponibilidad y calidad de imágenes en ciertos periodos
* El NDWI puede confundir áreas con vegetación acuática o suelos saturados
* Los resultados no deben interpretarse como mediciones hidrológicas exactas

No obstante, el enfoque es adecuado para analizar **tendencias y patrones a largo plazo**, que es el objetivo principal del proyecto.

---

## 7. Conclusiones

* La Observación de la Tierra es una herramienta eficaz para el análisis histórico de cuerpos de agua
* La consistencia metodológica es más importante que la maximización de resolución temporal
* El análisis espacial complementa y valida las series temporales
* EO permite apoyar, pero no reemplazar, mediciones oficiales e in situ

---

## 8. Trabajo futuro

Posibles extensiones del proyecto incluyen:

* Integrar datos de precipitación (por ejemplo, CHIRPS)
* Incorporar sensores SAR (Sentinel-1) para reducir el efecto de la nubosidad
* Ajustar umbrales dinámicos de NDWI
* Comparar resultados con datos hidrológicos oficiales

---

Este proyecto demuestra la capacidad de tomar decisiones metodológicas informadas, resolver problemas con datos incompletos y extraer conclusiones significativas a partir de información de Observación de la Tierra.


📧 Contact: bochicasimijaca@gmail.com

🔗 GitHub: https://github.com/Bochika
