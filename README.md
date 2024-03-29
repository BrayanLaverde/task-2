---
title: "Taller de R: Estadística y Programación"
author: "Brayan Laverde (202013972) - Philip Ramirez - Isabela Arcila"
date: "Abril 26 de 2022"
output: pdf_document
---
<!-- Configuración de la consola de R -->
```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = T , eval = T , warning = T)
```

En este taller se evalúan las clases 7 y 8 del curso. Se presentan 2 tipos de taller (A y B), pero usted solo debe desarrollar 1 de ellos. Para realizar este trabajo, podrá hacer grupo de hasta tres personas. Sea creativo en su código (no hay una respuesta única, todos los métodos que permitan obtener la misma respuesta son válidos). Cuando encuentre material de apoyo en línea que le permita solucionar algún problema, no olvide citar la fuente. Por último, lea atentamente las instrucciones del taller.

<!----------------------------------------------------------------------------->
## Instrucciones

* Este taller pesa el **25%** de la nota total del curso.

* No seguir las instrucciones tiene una penalización del **20%** de la nota final.

* El taller debe ser terminado antes de las 23:59 horas del 15 de mayo de 2022.

* En el repositorio asignado, debe incluir tres carpetas: input (datos originales), output (datos procesados) y code (script con la respuesta del taller).

* Debe escribir en el siguiente Excel [group-task.xlsx](\href{https://uniandes-my.sharepoint.com/:x:/g/personal/ef_martinezg_uniandes_edu_co/EVRAqeHLnEpEmlPTtvIApt8BXdxRDCGb3jIFLieUSAB8Yg) su código, su usuario de GitHub (por favor respetar mayúsculas y minúsculas) y en la columna grupo debe escribir un número que indique el grupo al cual pertenece (si va a desarrollar el task en grupo). 

* Por favor sea lo más organizado posible y comente paso a paso cada línea de código, pero recuerden **NO** usar ningún acento o carácter especial dentro del código para evitar problemas al abrir los scripts en los diferentes sistemas operativos.

* En las primeras líneas del script debe escribir su nombre, código y la versión de R sobre la que está trabajando.

* Para este taller debe usar al menos las librerías `pacman`, `rio` y `tidyverse`


<!----------------------------------------------------------------------------->
# Taller A

<!------------------->
## 1.Loops 

**1.0. Crear lista:** Cree un objeto tipo lista vacío, llámelo $chip$.

**1.1. Importar datos:** Use un loop para importar cada archivo .xlsx de $data/input$ en un elemento/posición diferente de $chip$. Esta lista debería 80 elementos (dataframes de la base de datos CHIP -Consolidador de Haciendas e información Pública- para los años 2017, 2018, 2019 y 2020).

<!------------------->
## 2. Funciones

**2.0. Crear función:** Cree una función que extraiga de un dataframe dentro de $chip$, el valor *PAGOS(Pesos)* para la categoría *EDUCACION*. Asegúrese de extraer el *código DANE* del municipio y el *periodo* de la información.

<!------------------->
## 3. Familia Apply

3.0. Aplique la función creada en el punto anterior a todos los elementos de la lista $chip$.
