# 📊 Análisis de disponibilidad de agua y saneamiento a nivel mundial

[![My Skills](https://go-skill-icons.vercel.app/api/icons?i=r,plotly,markdown)](https://go-skill-icons.vercel.app)

## 🧭 Tabla de contenidos

- [📌 Descripción general](#-descripción-general)
- [🎯 Objetivos del proyecto](#-objetivos-del-proyecto)
- [📁 Archivos del proyecto](#-archivos-del-proyecto)
- [🌐 Muestra visual del cuadro de mandos](#-muestra-visual-del-cuadro-de-mandos)
- [🖥️ Requisitos del sistema](#%EF%B8%8F-requisitos-del-sistema)
- [🧪 Instrucciones de reproducción de análisis](#-instrucciones-de-reproducción-de-análisis)
- [📚 Fuentes de datos](#-fuentes-de-datos)
- [🧾 Licencia](#-licencia)

## 📌 Descripción general

Este proyecto analiza el acceso al agua potable y los servicios de saneamiento a nivel global, con énfasis en las desigualdades entre regiones. Utilizando datos de la OMS, UNICEF e IHME entre 2000 y 2020, se aplican herramientas estadísticas y visualizaciones interactivas para detectar patrones, impactos sanitarios y zonas críticas.

---

### 🔍 Contexto y motivación

El agua es un recurso fundamental para la vida, pero su distribución y calidad no son equitativas. Millones de personas, especialmente en África y Asia, enfrentan diariamente dificultades para acceder a fuentes seguras y servicios básicos de saneamiento.

Estas carencias impactan directamente la salud pública, contribuyendo a enfermedades infecciosas, altas tasas de mortalidad y menor calidad de vida, especialmente en comunidades rurales y países de bajos ingresos.

El estudio no solo cuantifica el acceso, sino que explora la relación entre ingreso, localización (urbana/rural) y los indicadores sanitarios asociados. Gracias a mapas, series temporales y gráficos interactivos, se identifican zonas prioritarias de intervención.

El proyecto se alinea con los Objetivos de Desarrollo Sostenible (ODS), en especial el **ODS 6 (Agua limpia y saneamiento)**, y subraya la necesidad de políticas públicas eficaces y una mayor concienciación para asegurar el acceso universal al agua y saneamiento.

## 🎯 Objetivos del proyecto

**1. Realizar un análisis exhaustivo del acceso al agua potable y el saneamiento, abordando aspectos como la accesibilidad a fuentes seguras, la distribución geográfica y las consecuencias sanitarias asociadas a la carencia de estos servicios.**

**2. Generar conciencia sobre la escasez de agua en diversas partes del mundo, sensibilizando especialmente a las poblaciones que sí disponen de acceso, para fomentar el uso responsable del recurso y promover la equidad hídrica global.**

## 📁 Archivos del proyecto

### 📊 Datos

- **`nueva tabla v6.csv`**  
  Contiene datos estadísticos globales relacionados con el acceso a servicios de agua potable, saneamiento básico y su impacto en la salud, recopilados por entidades como **UNICEF** y **OMS**.

<details>
  <summary>📄 Ver estructura del archivo CSV</summary>

| Campo                                              | Descripción                                                    |
|----------------------------------------------------|----------------------------------------------------------------|
| Nombre del país o entidad                         | Nombre oficial del país o región                               |
| Código de país (ISO Alpha-3)                      | Código estándar de tres letras                                 |
| Año de los datos                                  | Año correspondiente                                            |
| Continente                                        | Ubicación geográfica                                           |
| Grupo de ingresos                                 | Según el Banco Mundial (ej. "Low income", "High income")       |
| Población sin agua mejorada                       | Número total sin acceso a fuentes de agua mejoradas            |
| Población sin saneamiento mejorado                | Número total sin acceso a instalaciones de saneamiento         |
| % defecación al aire libre                        | Porcentaje de la población                                     |
| % rural con acceso a agua potable básica          | Porcentaje de la población rural                               |
| % urbana con acceso a agua potable básica         | Porcentaje de la población urbana                              |
| Muertes por agua no segura                        | Estimación anual                                               |
| Muertes por saneamiento no seguro                 | Estimación anual                                               |
| Muertes por falta de acceso a lavado de manos     | Estimación anual                                               |
| Población total                                   | En el año correspondiente                                      |

</details>

---

### 📈 Análisis principal

- **`proyecto agua vfinal.Rmd`**  
  Archivo R Markdown que contiene el análisis completo y genera la memoria del proyecto.

  **Dependencias:**  
  `tidyverse`, `ggplot2`, `plotly`, `leaflet`, `highcharter`, `RColorBrewer`, `GGally`, `patchwork`, `openxlsx`, `pxR`, `dplyr`, `tidyr`, `fpp3`, `tsibble`, `urca`, `geojsonio`, `sf`, `wordcloud`, `knitr`, `htmltools`

- **`proyecto-agua-vfinal.html`**  
  Versión final renderizada de la memoria del proyecto.

---

### 📊 Visualización interactiva

- **`proyecto.agua.dashboard.Rmd`**  
  Dashboard interactivo creado con `flexdashboard` + `Shiny`.

---

### 🎨 Recursos visuales

- **`imagenes y css (1).zip`**  
  Archivos de imagen y estilos utilizados para personalizar la estética del dashboard y del informe. 

## 🌐 Muestra visual del cuadro de mandos

![](https://github.com/user-attachments/assets/51c39abb-43d3-4435-ba2d-6f121ac2b4ff)

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

- [Our World in Data – Water and Sanitation](https://ourworldindata.org/clean-water-sanitation)
  
  > Our World in Data recopila y publica información proveniente de fuentes oficiales como UNICEF, OMS y otras agencias internacionales.
- [IHME - Global Burden of Disease](https://www.healthdata.org/gbd)

Todos los datos utilizados son de acceso público y con fines educativos/investigativos.

## 🧾 Licencia 
Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

