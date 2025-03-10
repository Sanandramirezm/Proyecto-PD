# Proyecto de Procesamiento de Datos

## 📌 **Información del Proyecto**
**Clase:** Procesamiento de Datos  
**Profesor:** John Corredor  
**Integrantes del equipo:** Federico Quiroga, Ricardo Hurtado, Santiago Ramírez, Axel Caro

## 🎯 **Objetivo General**
El objetivo de este proyecto es analisar los resultados del examen ICFES en el departamento de Cundinamarca mediante factores determinantes como el acceso a internet, el nivel de pobreza y el nivel educativo. A partir de este análisis, se diseñará un plan de acción para fortalecer estos factores y optimizar el desempeño académico en la región.

Cundinamarca es el tercer departamento más poblado de Colombia con aproximadamente 3.5 millones de habitantes. En 2023, registró el índice de pobreza más bajo del país (21.5%) y en 2024 se destinaron 72 mil millones de pesos para mejorar su infraestructura educativa. Además, el 68% de los hogares cuenta con conexión a internet, lo que lo ubica entre los departamentos con mayor acceso a este servicio.

## 📊 **Conjuntos de Datos Seleccionados**
Se utilizaron dos conjuntos de datos extraídos de la página oficial del ICFES ([Resultados ICFES](https://www.icfes.gov.co/evaluaciones-icfes/resultados/)) correspondientes al primer y segundo semestre de 2023.

Estos conjuntos incluyen variables clave como:
- Resultados en las pruebas Saber 11
- Nivel educativo de los padres
- Área de residencia
- Acceso a internet
- Estrato socioeconómico

La variedad de estas variables permite un análisis integral y detallado.

## 📈 **Gráficas y Estadísticos**
Las visualizaciones generadas para el análisis incluyen:
1. **Histograma de puntajes**
2. **Boxplot de puntajes por estrato socioeconómico**
3. **Gráfico de barras del nivel educativo de los padres**
4. **Gráfico de dispersión entre número de libros en el hogar y puntajes**
5. **Distribución de estudiantes por municipio de residencia**

Las tablas generadas incluyen:
- **Tabla 1 & 2:** Promedio de puntajes y relación entre uso de internet y desempeño académico.
- **Tabla 3:** Estadísticos descriptivos generales.

## 🔍 **Reporte de Calidad de Datos**
Para evaluar la calidad de los datos, se realizó un análisis de valores faltantes, siguiendo estos pasos:
- Carga del archivo `SB11_20231.TXT` usando `pandas`.
- Cálculo del número total y porcentaje de valores faltantes por variable.
- Generación de una tabla resumen con los resultados.

### 🔧 **Limpieza y Transformación de Datos**
El dataset `SB11_20231` se limpió y transformó asegurando calidad y completitud. Algunas de las acciones tomadas incluyen:
- **Imputación de valores nulos**:
  - Variables categóricas: Se imputaron usando la moda.
  - Variables numéricas: Se reemplazaron por la media dentro de grupos.
- **Conversión de datos**:
  - Variables categóricas a numéricas.
  - Variables binarias convertidas a 1 y 0.
- **Detección de valores atípicos**:
  - Se aplicó el rango intercuartil (IQR) y visualización mediante histogramas.

## 🔬 **Preguntas de Investigación**
1. ¿Existe correlación entre acceso a internet en el hogar y el puntaje global del ICFES?
2. ¿Cómo influye el nivel educativo de los padres en el desempeño de los estudiantes?
3. ¿El estrato socioeconómico tiene un impacto significativo en los resultados?
4. ¿Los estudiantes de colegios privados obtienen mejores puntajes que los de colegios públicos?
5. ¿Cuáles municipios tienen los promedios más altos y más bajos?
6. ¿Existe relación entre la cantidad de libros en el hogar y la lectura crítica?
7. ¿El tiempo de uso de internet influye en los resultados de matemáticas y ciencias naturales?
8. ¿Qué características socioeconómicas comparten los estudiantes con mejores puntajes?

## 📚 **Fuentes**
- [DANE - Estadísticas de pobreza](https://www.dane.gov.co/index.php/estadisticas-por-tema/pobreza-y-condiciones-de-vida/pobreza-monetaria)
- [Cundinamarca - Infraestructura educativa](https://www.cundinamarca.gov.co/noticias/cerca-de-17-mil-estudiantes-de-cundinamarca-se-benefician-con-el-mejoramiento-de-la-infraestructura-educativa)
- [Conectividad a internet en Cundinamarca](https://www.cundinamarca.gov.co/wcm/connect/e9c7448e-bb4e-4dba-8992-a725eae2597d/indicador_hogares+que+poseen+conexi%C3%B3n+a+Internet.pdf?MOD=AJPERES&CONVERT_TO=url&CACHEID=ROOTWORKSPACE-e9c7448e-bb4e-4dba-8992-a725eae2597d-p8cQ3LZ)
- [Resultados ICFES](https://www.icfes.gov.co/evaluaciones-icfes/resultados/)

