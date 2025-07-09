# 📊 Análisis de disponibilidad de agua y saneamiento a nivel mundial

[![My Skills](https://go-skill-icons.vercel.app/api/icons?i=r,plotly,markdown)](https://go-skill-icons.vercel.app)

## Descripción general
Este proyecto aborda de manera integral la problemática del acceso al agua potable y los servicios de saneamiento a nivel global, con un enfoque especial en las desigualdades geográficas, económicas y sociales que persisten en distintas regiones del mundo. Utilizando datos oficiales de organismos internacionales como la OMS, UNICEF y el IHME, el análisis cubre el periodo 2000-2020 y se apoya en herramientas estadísticas y visualizaciones interactivas para facilitar la interpretación de los resultados.

El agua es un recurso fundamental para la vida, pero su distribución y calidad no son equitativas. Millones de personas, especialmente en África y Asia, enfrentan diariamente dificultades para acceder a fuentes seguras de agua potable y a instalaciones de saneamiento adecuadas. Estas carencias tienen un impacto directo en la salud pública, contribuyendo a la propagación de enfermedades infecciosas, altas tasas de mortalidad y una menor calidad de vida, sobre todo en comunidades rurales y países de bajos ingresos.

El estudio no solo cuantifica el acceso y la falta de servicios, sino que también explora la relación entre nivel de ingresos, localización (urbana/rural) y los principales indicadores sanitarios asociados al agua y al saneamiento. Mediante mapas, series temporales y diagramas interactivos, se identifican patrones, tendencias y zonas críticas donde la intervención es más urgente.

Además, el proyecto destaca la importancia de la sostenibilidad y la gestión eficiente de los recursos hídricos, alineándose con los Objetivos de Desarrollo Sostenible (ODS) de Naciones Unidas, en particular el ODS 6 (Agua limpia y saneamiento). Se enfatiza la necesidad de políticas públicas efectivas y de una mayor concienciación social para garantizar que el acceso al agua y al saneamiento sea un derecho universal, no un privilegio.

## 📁 Archivos del proyecto
`nueva tabla v6.csv`: Este archivo CSV contiene datos estadísticos globales relacionados con el acceso a servicios de agua potable, saneamiento básico y su impacto en la salud, recopilados por entidades como UNICEF o la OMS. A continuación, se detalla su estructura y contenido:

- Nombre del país o entidad
- Código de país (ISO Alpha-3)
- Año de los datos
- Continente al que pertenece el país
- Grupo de ingresos según el Banco Mundial (ej. "Low income", "High income")
- Población total sin acceso a fuentes de agua mejoradas
- Población total sin acceso a instalaciones de saneamiento mejoradas
- Porcentaje de la población que practica la defecación al aire libre
- Porcentaje de la población rural con acceso a servicios básicos de agua potable
- Porcentaje de la población urbana con acceso a servicios básicos de agua potable
- Muertes atribuidas al consumo de agua no segura
- Muertes atribuidas a saneamiento no seguro
- Muertes por falta de acceso a lavado de manos
- Población total del país/entidad en el año correspondiente

`proyecto agua vfinal.Rmd`: Archivo R Markdown principal que contiene el código y análisis completo para generar la memoria del proyecto. 
- Dependencias: `tidyverse`, `ggplot2`, `plotly`, `leaflet`, `highcharter`, `RColorBrewer`, `GGally`, `patchwork`, `openxlsx`, `pxR`, `dplyr`, `tidyr`, `fpp3`, `tsibble`, `urca`, `geojsonio`, `sf`, `wordcloud`, `knitr`, `htmltools`

`proyecto-agua-vfinal.html`: Memoria del proyecto.

`proyecto.agua.dashboard.Rmd`: Dashboard interactivo en R Markdown (flexdashboard + Shiny). 

Captura de muestra:
<br><br>
![FireShot Capture 001 - Estadísticas sobre agua potable y saneamiento -  127 0 0 1](https://github.com/user-attachments/assets/b5df7882-4154-468f-b19c-f11a525018d9)

`imagenes y css (1).zip`: Se incluyen algunos recursos visuales y de estilo para mejorar la estética de los resultados generados. 

## 🖥️ Requisitos del sistema

- R ≥ 4.1
- RStudio 
- Conexión a internet (algunos paquetes descargan dependencias externas)
- Sistema operativo compatible con bibliotecas geoespaciales (`sf`, `leaflet`)

## 🧪 Instrucciones de reproducción de análisis
1. Descomprimir `imagenes y css (1).zip` en la misma carpeta donde se encuentren los archivos `.Rmd`
2. Acceder a `proyecto agua vfinal.Rmd` mediante RStudio y hacer click en `Knit`, para generar el informe deseado.
3. Para consultar el dashboard, abrir `proyecto.agua.dashboard.Rmd` y clicar en `Run Document`.

_* Todos los archivos del repositorio deben estar en la misma carpeta._

## 📚 Fuentes de datos

- [Our World in Data – Water and Sanitation](https://ourworldindata.org/water-access)
  
  > Our World in Data recopila y publica información proveniente de fuentes oficiales como UNICEF, OMS y otras agencias internacionales.
- [IHME - Global Burden of Disease](https://www.healthdata.org/gbd)

Todos los datos utilizados son de acceso público y con fines educativos/investigativos.

## 🧾 Licencia 
Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.







