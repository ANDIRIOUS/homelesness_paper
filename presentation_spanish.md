# El Impacto del Aumento de los Alquileres en la Falta de Vivienda en Áreas Urbanas de los Estados Unidos

## Presentación de Investigación

---

## Introducción

### Pregunta de Investigación
- ¿En qué medida los aumentos en los precios de alquiler afectan causalmente las tasas de falta de vivienda en áreas urbanas de los Estados Unidos?

### Importancia
- La falta de vivienda sigue siendo un desafío social persistente en los Estados Unidos
- Los costos de vivienda han aumentado dramáticamente durante la última década
- Comprender las relaciones causales es crucial para intervenciones políticas efectivas

---

## Revisión de Literatura

### Marco Teórico
- O'Flaherty (1995): La falta de vivienda resulta de una combinación de pobreza y condiciones del mercado de vivienda
- La teoría predice que los aumentos en el alquiler aumentarían las tasas de falta de vivienda

### Evidencia Empírica
- Quigley, Raphael, y Smolensky (2001): Un aumento del 10% en el alquiler asociado con un aumento del 13.6% en la falta de vivienda
- Glynn y Fox (2019): Las tasas de falta de vivienda aumentan bruscamente cuando el alquiler medio supera el 32% del ingreso medio
- Evans, Sullivan, y Wallskog (2016): Los aumentos de alquiler causados por el auge del fracking afectaron la falta de vivienda

---

## Desafíos Metodológicos

### Preocupaciones de Endogeneidad
- Los precios de alquiler y las tasas de falta de vivienda pueden estar determinados simultáneamente
- Podría existir causalidad inversa
- Factores no observados podrían afectar ambas variables

### Nuestro Enfoque
- Metodología de variables instrumentales (IV)
- Utilizando el alquiler en áreas adyacentes de Continuum of Care (CoC) del año anterior como nuestro instrumento
- Controles para factores socioeconómicos (desempleo, pobreza)

---

## Fuentes de Datos

- **Datos de Falta de Vivienda**: Informe de Evaluación de Personas sin Hogar Anual 2024 (AHAR) de HUD
- **Datos de Alquiler**: Datos de Alquiler de Mercado Justo (FMR) para 2024 de HUD
- **Variables Socioeconómicas**: 
  - Datos de desempleo a nivel de condado de BLS
  - Estadísticas de pobreza de la Encuesta de la Comunidad Americana (ACS) de la Oficina del Censo
- **Datos Geográficos**: Información sobre áreas adyacentes de CoC

---

## Metodología

### Enfoque de Variables Instrumentales

Primera etapa:
$Alquiler_i = \alpha_0 + \alpha_1 AlquilerAdyacente_{i-1} + \alpha_2 X_i + \nu_i$

Segunda etapa:
$FaltaDeVivienda_i = \beta_0 + \beta_1 \widehat{Alquiler_i} + \beta_2 X_i + \epsilon_i$

- Supuesto clave de identificación: Los alquileres de áreas adyacentes afectan la falta de vivienda solo a través de los alquileres actuales

---

## Estadísticas Descriptivas

![Distribución de Precios Promedio de Alquiler](/home/ubuntu/analysis/figures/figure1_rent_distribution.png)

---

## Relación Entre Alquiler y Falta de Vivienda

![Relación Entre Alquiler y Tasa de Falta de Vivienda](/home/ubuntu/analysis/figures/figure2_rent_homelessness.png)

---

## Relación Entre Alquiler y Factores Socioeconómicos

![Relación Entre Alquiler y Tasa de Desempleo](/home/ubuntu/analysis/figures/figure3_rent_unemployment.png)

---

## Relación Entre Alquiler y Pobreza

![Relación Entre Alquiler y Tasa de Pobreza](/home/ubuntu/analysis/figures/figure4_rent_poverty.png)

---

## Resultados de Primera Etapa

![Regresión de Primera Etapa - Relevancia del Instrumento](/home/ubuntu/analysis/figures/figure5_first_stage.png)

- Fuerte correlación entre el instrumento y los precios de alquiler
- Estadístico F: 42.7 (muy por encima del umbral de 10)
- R-cuadrado: 0.64

---

## Resultados Principales

![Comparación de Estimaciones OLS e IV](/home/ubuntu/analysis/figures/figure6_ols_iv_comparison.png)

- Estimación OLS: Aumento de $100 en alquiler → aumento de 0.023 puntos porcentuales en falta de vivienda
- Estimación IV: Aumento de $100 en alquiler → aumento de 0.058 puntos porcentuales en falta de vivienda
- Estimaciones IV mayores que OLS, sugiriendo que OLS subestima el verdadero efecto causal

---

## Resultados Transformados Logarítmicamente

- Interpretación de elasticidad: Aumento del 10% en alquiler → aumento del 7.2% en falta de vivienda
- Efecto más fuerte en ciudades de alto costo (elasticidad de 0.85) comparado con ciudades de costo moderado (elasticidad de 0.61)
- Resultados robustos a varias especificaciones de modelos

---

## Implicaciones Políticas

### Oferta de Vivienda
- Aumentar la oferta de vivienda asequible
- Zonificación inclusiva
- Incentivos fiscales para el desarrollo de vivienda asequible
- Inversiones en vivienda pública

### Asistencia de Alquiler
- Vales de vivienda para reducir la carga de alquiler para hogares de bajos ingresos
- Incluso reducciones modestas en los costos de alquiler podrían reducir significativamente la falta de vivienda

### Intervenciones Dirigidas
- Se necesitan intervenciones más fuertes en ciudades de alto costo
- Medidas de control de alquiler
- Requisitos más altos de vivienda asequible para nuevos desarrollos

---

## Limitaciones

- El supuesto de variables instrumentales podría ser violado si existen efectos de derrame
- Los conteos de Point-in-Time pueden subestimar la población sin hogar
- Los resultados pueden no generalizarse a contextos rurales o suburbanos
- Limitaciones de datos en la medición de características de áreas adyacentes

---

## Conclusión

- Fuerte evidencia de que los aumentos de alquiler afectan causalmente las tasas de falta de vivienda
- Un aumento del 10% en el alquiler asociado con un aumento del 7.2% en la falta de vivienda
- Abordar la asequibilidad de la vivienda es crucial para reducir la falta de vivienda
- Cuantificar esta relación proporciona información valiosa para los formuladores de políticas

---

## Gracias

### ¿Preguntas?

Contacto: [Su Información de Contacto]
