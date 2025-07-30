---
permalink: /cv/
title: "Currículum Vitae"
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Experiencia Profesional

### Operador CNC
**IDEI** (2022 - Presente)  
- Operación y programación de fresadoras CNC
- Fabricación de componentes industriales

### Asistente de Investigación
**Laboratorio de Genética Forestal - UJED** (2020 - Presente)  
- Análisis bioinformático de datos genómicos
- Desarrollo de scripts Python/R para procesamiento de datos
- Limpieza y gestión de bases de datos PostgreSQL

## Educación

### Doctorado en Ciencias Agropecuarias y Forestales
**Universidad Juárez del Estado de Durango** (2023 - Presente)  
- Sistemas de monitoreo remoto con IoT
- Análisis de datos para agricultura de precisión

### Maestría en Ingeniería
**Instituto Tecnológico del Valle del Guadiana** (2020 - 2022)  
4.0/4.0 | Especialización en sistemas mecatrónicos

## Habilidades Técnicas

| Categoría          | Tecnologías                                      |
|--------------------|-------------------------------------------------|
| Programación       | Python, R, SQL, C++, LabVIEW, Arduino/ESP32     |
| GIS & Agricultura  | QGIS, ArcGIS, Sensores agrícolas, Análisis de suelos |
| Manufactura        | SolidWorks, CNC, Fusion 360, Impresión 3D       |
| Ciencia de Datos   | Machine Learning, Pandas, Scikit-learn, TensorFlow |

## Publicaciones

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}