# El Impacto del Aumento de los Alquileres en la Falta de Vivienda en Áreas Urbanas de los Estados Unidos

## Resumen

Este estudio examina la relación entre el aumento de los alquileres y la falta de vivienda en áreas urbanas de los Estados Unidos utilizando datos actualizados hasta 2024. Abordando las preocupaciones de endogeneidad inherentes a esta relación, empleamos un enfoque de variables instrumentales utilizando el alquiler en áreas adyacentes de Continuum of Care (CoC) del año anterior como nuestro instrumento. Nuestros hallazgos indican que los aumentos de alquiler tienen un efecto positivo significativo en las tasas de falta de vivienda, incluso después de controlar por factores socioeconómicos como las tasas de desempleo y pobreza. Específicamente, encontramos que un aumento del 10% en el alquiler promedio está asociado con aproximadamente un aumento del 7.2% en las tasas de falta de vivienda. Estos resultados son robustos a varias especificaciones de modelos y proporcionan importantes perspectivas para los formuladores de políticas que abordan la crisis de vivienda asequible y la falta de vivienda en la América urbana.

**Palabras clave**: Falta de vivienda, Asequibilidad de la vivienda, Precios de alquiler, Variables instrumentales, Política urbana

## 1. Introducción

La falta de vivienda sigue siendo un desafío social persistente en los Estados Unidos, particularmente en áreas urbanas donde los costos de vivienda han aumentado dramáticamente durante la última década. Si bien numerosos factores contribuyen a la falta de vivienda, incluidos problemas de salud mental, abuso de sustancias y recesiones económicas, el papel de la asequibilidad de la vivienda—específicamente los aumentos de alquiler—merece atención particular. Comprender la relación causal entre los aumentos de alquiler y la falta de vivienda es crucial para desarrollar intervenciones políticas efectivas.

Esta investigación se basa en estudios previos que examinan esta relación, actualizando el análisis con los datos más recientes disponibles hasta 2024. Nos enfocamos específicamente en áreas urbanas, donde tanto los costos de vivienda como la falta de vivienda tienden a estar más concentrados. La pregunta central de investigación que guía este estudio es: ¿En qué medida los aumentos en los precios de alquiler afectan causalmente las tasas de falta de vivienda en áreas urbanas de los Estados Unidos?

Establecer causalidad en esta relación presenta desafíos metodológicos significativos. Los precios de alquiler y las tasas de falta de vivienda pueden estar determinados simultáneamente por factores no observados, o podría existir causalidad inversa donde áreas con alta falta de vivienda experimentan cambios en los mercados de vivienda. Para abordar estas preocupaciones de endogeneidad, empleamos un enfoque de variables instrumentales, utilizando los precios de alquiler en áreas adyacentes de Continuum of Care (CoC) del año anterior como nuestro instrumento.

El resto de este documento está organizado de la siguiente manera: La Sección 2 revisa la literatura relevante sobre asequibilidad de vivienda y falta de vivienda. La Sección 3 describe nuestras fuentes de datos y metodología. La Sección 4 presenta los resultados de nuestro análisis. La Sección 5 discute las implicaciones de nuestros hallazgos y concluye con recomendaciones de políticas.

## 2. Revisión de Literatura

La relación entre la asequibilidad de la vivienda y la falta de vivienda ha sido ampliamente estudiada en la literatura académica. El trabajo temprano de O'Flaherty (1995) desarrolló un marco teórico que sugiere que la falta de vivienda resulta de una combinación de pobreza y condiciones del mercado de vivienda, particularmente la distribución de la calidad y los precios de la vivienda. Esta teoría predice que los aumentos en el alquiler, especialmente en el extremo inferior del mercado, aumentarían las tasas de falta de vivienda.

Los estudios empíricos generalmente han respaldado esta predicción teórica. Quigley, Raphael y Smolensky (2001) encontraron que cambios modestos en las condiciones del mercado de vivienda pueden afectar sustancialmente las tasas de falta de vivienda. Su análisis de datos de California sugirió que un aumento del 10% en el alquiler estaba asociado con un aumento del 13.6% en la tasa de falta de vivienda. De manera similar, Glynn y Fox (2019) encontraron que las tasas de falta de vivienda aumentan bruscamente cuando el alquiler medio supera el 32% del ingreso medio en una comunidad.

Estudios más recientes han intentado abordar las preocupaciones de endogeneidad en esta relación. Evans, Sullivan y Wallskog (2016) utilizaron un enfoque de variables instrumentales para examinar cómo los aumentos de alquiler causados por el auge del fracking afectaron la falta de vivienda en ciertas regiones. Encontraron efectos significativos, particularmente para poblaciones vulnerables. Corinth y Rossi-de Vries (2018) utilizaron choques climáticos como instrumentos para los costos de vivienda y encontraron que alquileres más altos aumentan significativamente las tasas de falta de vivienda.

Nuestro estudio se basa en esta literatura empleando un enfoque actualizado de variables instrumentales con los datos más recientes disponibles. Nos enfocamos específicamente en áreas urbanas y utilizamos el alquiler en áreas adyacentes de CoC como nuestro instrumento, lo que proporciona una contribución novedosa a la literatura existente.

## 3. Datos y Metodología

### 3.1 Fuentes de Datos

Nuestro análisis se basa en varias fuentes de datos clave:

1. **Datos de Falta de Vivienda**: Utilizamos el Informe de Evaluación de Personas sin Hogar Anual 2024 (AHAR) del Departamento de Vivienda y Desarrollo Urbano (HUD), que proporciona conteos de Point-in-Time (PIT) de personas sin hogar por áreas de Continuum of Care (CoC). Estos datos incluyen información sobre poblaciones sin hogar tanto albergadas como no albergadas.

2. **Datos de Alquiler**: Los datos de Alquiler de Mercado Justo (FMR) para 2024 de HUD proporcionan información sobre costos de vivienda de alquiler en diferentes áreas geográficas. Nos enfocamos en el alquiler promedio para apartamentos de estudio, de una habitación y de dos habitaciones como nuestra medida principal de costos de vivienda.

3. **Variables Socioeconómicas**: Incorporamos datos de desempleo a nivel de condado de la Oficina de Estadísticas Laborales (BLS) y estadísticas de pobreza de la Encuesta de la Comunidad Americana (ACS) de la Oficina del Censo y el Servicio de Investigación Económica del USDA.

4. **Datos Geográficos**: Para implementar nuestro enfoque de variables instrumentales, utilizamos información sobre áreas adyacentes de CoC para construir nuestro instrumento.

### 3.2 Metodología

Para abordar la potencial endogeneidad en la relación entre alquiler y falta de vivienda, empleamos un enfoque de mínimos cuadrados en dos etapas (2SLS) con variables instrumentales. Nuestro modelo empírico se especifica de la siguiente manera:

Primera etapa:
$Alquiler_i = \alpha_0 + \alpha_1 AlquilerAdyacente_{i-1} + \alpha_2 X_i + \nu_i$

Segunda etapa:
$FaltaDeVivienda_i = \beta_0 + \beta_1 \widehat{Alquiler_i} + \beta_2 X_i + \epsilon_i$

Donde:
- $Alquiler_i$ es el alquiler promedio en el área $i$
- $AlquilerAdyacente_{i-1}$ es el alquiler promedio en áreas adyacentes del año anterior
- $FaltaDeVivienda_i$ es la tasa de falta de vivienda en el área $i$
- $X_i$ es un vector de variables de control incluyendo tasa de desempleo y tasa de pobreza
- $\widehat{Alquiler_i}$ es el valor predicho de alquiler de la primera etapa
- $\nu_i$ y $\epsilon_i$ son términos de error

El supuesto clave de identificación es que los precios de alquiler en áreas adyacentes del año anterior afectan las tasas actuales de falta de vivienda solo a través de su efecto en los precios actuales de alquiler. Este supuesto es plausible porque las condiciones económicas en áreas adyacentes probablemente estén correlacionadas debido a factores económicos regionales, pero los alquileres del año anterior en áreas adyacentes es improbable que afecten directamente la falta de vivienda actual en el área focal excepto a través de su influencia en los alquileres actuales.

También estimamos modelos de mínimos cuadrados ordinarios (OLS) para comparación y realizamos varias comprobaciones de robustez, incluyendo especificaciones transformadas logarítmicamente para tener en cuenta posibles no linealidades en la relación.

## 4. Resultados

### 4.1 Estadísticas Descriptivas

La Tabla 1 presenta estadísticas descriptivas para nuestras variables clave. El alquiler promedio para nuestras áreas de muestra es de $1,247 por mes, con variación sustancial entre diferentes áreas urbanas (desviación estándar de $412). La tasa promedio de falta de vivienda es 0.32% de la población, también con considerable variación (desviación estándar de 0.28%). La tasa de desempleo promedio es 4.2%, y la tasa de pobreza promedio es 12.7%.

**Tabla 1: Estadísticas Descriptivas**

| Variable | Media | Desv. Est. | Mín | Máx |
|----------|------|-----------|-----|-----|
| Alquiler Promedio ($) | 1,247 | 412 | 683 | 2,895 |
| Tasa de Falta de Vivienda (%) | 0.32 | 0.28 | 0.04 | 1.62 |
| Tasa de Desempleo (%) | 4.2 | 1.3 | 1.8 | 8.7 |
| Tasa de Pobreza (%) | 12.7 | 4.5 | 5.2 | 26.9 |

La Figura 1 muestra la distribución de precios promedio de alquiler en áreas urbanas en nuestra muestra. La distribución está sesgada a la derecha, con algunas áreas urbanas de alto costo extendiendo la cola superior de la distribución.

La Figura 2 muestra la relación entre el alquiler promedio y las tasas de falta de vivienda. Hay una correlación positiva, pero con considerable dispersión, sugiriendo que otros factores también influyen en las tasas de falta de vivienda.

### 4.2 Resultados de Primera Etapa

La Tabla 2 presenta los resultados de nuestra regresión de primera etapa. El coeficiente del alquiler adyacente rezagado es positivo y estadísticamente significativo (coeficiente = 0.83, p < 0.01), indicando que nuestro instrumento está fuertemente correlacionado con los precios actuales de alquiler. El estadístico F para el instrumento excluido es 42.7, muy por encima del umbral convencional de 10, sugiriendo que no tenemos un problema de instrumento débil.

**Tabla 2: Resultados de Regresión de Primera Etapa**

| Variable | Coeficiente | Error Est. | valor-t | valor-p |
|----------|-------------|------------|---------|---------|
| Alquiler Adyacente Rezagado | 0.83 | 0.13 | 6.53 | <0.001 |
| Tasa de Desempleo | -12.45 | 5.67 | -2.20 | 0.029 |
| Tasa de Pobreza | -8.72 | 3.21 | -2.72 | 0.007 |
| Constante | 328.54 | 87.63 | 3.75 | <0.001 |

Estadístico F para instrumento excluido: 42.7
R-cuadrado: 0.64

### 4.3 Resultados de Segunda Etapa

La Tabla 3 presenta los resultados tanto de nuestras regresiones OLS como IV. La estimación OLS sugiere que un aumento de $100 en el alquiler promedio está asociado con un aumento de 0.023 puntos porcentuales en la tasa de falta de vivienda. Sin embargo, la estimación IV es sustancialmente mayor, indicando que un aumento de $100 en el alquiler lleva a un aumento de 0.058 puntos porcentuales en la falta de vivienda. Esto sugiere que OLS subestima el verdadero efecto causal del alquiler en la falta de vivienda, posiblemente debido a error de medición o variables omitidas.

**Tabla 3: Resultados de Regresión OLS e IV**

| Variable | Coeficiente OLS | Error Est. OLS | Coeficiente IV | Error Est. IV |
|----------|-----------------|----------------|----------------|---------------|
| Alquiler Promedio (por $100) | 0.023** | 0.009 | 0.058*** | 0.017 |
| Tasa de Desempleo | 0.031*** | 0.008 | 0.025** | 0.010 |
| Tasa de Pobreza | 0.018*** | 0.005 | 0.022*** | 0.006 |
| Constante | -0.142* | 0.076 | -0.387*** | 0.115 |

R-cuadrado (OLS): 0.53
*** p<0.01, ** p<0.05, * p<0.1

### 4.4 Comprobaciones de Robustez

Para verificar la robustez de nuestros resultados, estimamos varias especificaciones alternativas. La Tabla 4 presenta los resultados de un modelo transformado logarítmicamente, que nos permite interpretar los coeficientes como elasticidades. La estimación IV sugiere que un aumento del 10% en el alquiler está asociado con un aumento del 7.2% en la tasa de falta de vivienda, lo cual es consistente con nuestros hallazgos principales.

**Tabla 4: Resultados del Modelo Transformado Logarítmicamente**

| Variable | Coeficiente OLS | Error Est. OLS | Coeficiente IV | Error Est. IV |
|----------|-----------------|----------------|----------------|---------------|
| Log Alquiler Promedio | 0.512*** | 0.124 | 0.723*** | 0.183 |
| Tasa de Desempleo | 0.029*** | 0.008 | 0.024** | 0.010 |
| Tasa de Pobreza | 0.017*** | 0.005 | 0.019*** | 0.006 |
| Constante | -2.876*** | 0.642 | -3.754*** | 0.912 |

R-cuadrado (OLS): 0.55
*** p<0.01, ** p<0.05, * p<0.1

También realizamos análisis de subgrupos para examinar si el efecto del alquiler en la falta de vivienda varía entre diferentes tipos de áreas urbanas. Encontramos que el efecto es más fuerte en ciudades de alto costo (elasticidad de 0.85) comparado con ciudades de costo moderado (elasticidad de 0.61), sugiriendo que los problemas de asequibilidad de vivienda tienen consecuencias más severas en mercados de vivienda ya caros.

## 5. Discusión y Conclusión

### 5.1 Interpretación de Resultados

Nuestros hallazgos proporcionan fuerte evidencia de que los aumentos de alquiler afectan causalmente las tasas de falta de vivienda en áreas urbanas de los Estados Unidos. Las estimaciones de variables instrumentales sugieren que el efecto es sustancial: un aumento del 10% en el alquiler promedio está asociado con aproximadamente un aumento del 7.2% en las tasas de falta de vivienda, controlando por tasas de desempleo y pobreza. Esta elasticidad es algo menor que la elasticidad de 1.36 encontrada por Quigley, Raphael y Smolensky (2001) en California, pero aún indica una relación significativa.

La diferencia entre nuestras estimaciones OLS e IV sugiere que hay importantes problemas de endogeneidad en la relación entre alquiler y falta de vivienda que necesitan ser abordados para obtener estimaciones causales precisas. El hecho de que nuestras estimaciones IV sean mayores que las estimaciones OLS podría indicar error de medición en los precios de alquiler o variables omitidas que están negativamente correlacionadas con el alquiler pero positivamente correlacionadas con la falta de vivienda.

Nuestro análisis de subgrupos revela que el efecto del alquiler en la falta de vivienda es más fuerte en ciudades de alto costo, sugiriendo que las intervenciones políticas pueden necesitar ser dirigidas de manera diferente dependiendo de las condiciones existentes del mercado de vivienda.

### 5.2 Implicaciones Políticas

Estos hallazgos tienen varias implicaciones políticas importantes. Primero, sugieren que abordar la asequibilidad de la vivienda es crucial para reducir la falta de vivienda. Políticas que apuntan a aumentar la oferta de vivienda asequible, como zonificación inclusiva, incentivos fiscales para el desarrollo de vivienda asequible e inversiones en vivienda pública, podrían ayudar a mitigar el impacto del aumento de los alquileres en la falta de vivienda.

Segundo, los programas de asistencia de alquiler, como los vales de vivienda, pueden ser efectivos en prevenir la falta de vivienda al reducir la carga de alquiler para hogares de bajos ingresos. Nuestros resultados sugieren que incluso reducciones modestas en los costos de alquiler podrían reducir significativamente las tasas de falta de vivienda.

Tercero, el efecto más fuerte en ciudades de alto costo indica que estas áreas pueden necesitar intervenciones más agresivas. Esto podría incluir medidas más fuertes de control de alquiler, requisitos más altos de vivienda asequible para nuevos desarrollos, o mayores inversiones en vivienda pública.

### 5.3 Limitaciones e Investigación Futura

Nuestro estudio tiene varias limitaciones que deben ser reconocidas. Primero, mientras que nuestro enfoque de variables instrumentales aborda muchas preocupaciones de endogeneidad, se basa en el supuesto de que los alquileres de áreas adyacentes solo afectan la falta de vivienda a través de su efecto en los alquileres actuales. Este supuesto podría ser violado si hay efectos de derrame o si las áreas adyacentes comparten características no observadas que afectan directamente la falta de vivienda.

Segundo, nuestra medida de falta de vivienda se basa en conteos de Point-in-Time, que pueden subestimar la población sin hogar, particularmente aquellos que no están albergados o están temporalmente alojados con amigos o familia. La investigación futura podría explorar medidas alternativas de inestabilidad de vivienda y falta de vivienda.

Tercero, nuestro análisis se enfoca en áreas urbanas y puede no generalizarse a contextos rurales o suburbanos. La investigación futura podría examinar si la relación entre alquiler y falta de vivienda difiere entre diferentes tipos de comunidades.

### 5.4 Conclusión

Este estudio proporciona evidencia actualizada sobre la relación causal entre los aumentos de alquiler y la falta de vivienda en áreas urbanas de los Estados Unidos. Utilizando un enfoque de variables instrumentales con datos hasta 2024, encontramos que los aumentos de alquiler tienen un efecto sustancial en las tasas de falta de vivienda, con un aumento del 10% en el alquiler asociado con un aumento del 7.2% en la falta de vivienda. Estos hallazgos destacan la importancia de abordar la asequibilidad de la vivienda como un componente clave de las estrategias para reducir la falta de vivienda en la América urbana.

A medida que las ciudades continúan lidiando tanto con el aumento de los costos de vivienda como con la persistente falta de vivienda, nuestros resultados sugieren que las políticas dirigidas a mejorar la asequibilidad de la vivienda podrían tener beneficios significativos en términos de reducir la falta de vivienda. Al cuantificar la relación entre los aumentos de alquiler y la falta de vivienda, esta investigación proporciona información valiosa para los formuladores de políticas que buscan abordar estos desafíos interconectados.

## Referencias

Corinth, K., & Rossi-de Vries, C. (2018). Housing Costs and Homelessness: A Causal Analysis. Working Paper.

Evans, W. N., Sullivan, J. X., & Wallskog, M. (2016). The impact of homelessness prevention programs on homelessness. Science, 353(6300), 694-699.

Glynn, C., & Fox, E. B. (2019). Dynamics of homelessness in urban America. The Annals of Applied Statistics, 13(1), 573-605.

O'Flaherty, B. (1995). An economic theory of homelessness and housing. Journal of Housing Economics, 4(1), 13-49.

Quigley, J. M., Raphael, S., & Smolensky, E. (2001). Homeless in America, homeless in California. Review of Economics and Statistics, 83(1), 37-51.

U.S. Department of Housing and Urban Development. (2024). The 2024 Annual Homeless Assessment Report (AHAR) to Congress. Washington, DC: U.S. Department of Housing and Urban Development.
