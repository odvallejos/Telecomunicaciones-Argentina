## <center>Proyecto Individual 03 - Data Analytics</center>

# <center>**Telecomunicaciones**</center>

## <center>Daniel Vallejos</center>

---

# Contexto

La industria de las telecomunicaciones ha jugado un papel vital en nuestra sociedad, facilitando la información a escala internacional y permitiendo la comunicación continua incluso en medio de una pandemia mundial. La transferencia de datos y comunicación se realiza en su mayoría a través de internet, líneas telefónicas fijas, telefonía móvil, casi en cualquier lugar del mundo.

En comparación con la media mundial, Argentina está a la vanguardia del desarrollo de las telecomunicaciones, teniendo para el 2020 un total de 62,12 millones conexiones.

# Desarrollo

Se procedió al Análisis Exploratorio de los Datos (EDA) con los datos provistos desde el sitio web de ENACOM<br/>

**Acceso a Internet:** *Información de mercado, oferta, demanda y cobertura de los servicios de comunicaciones* <br/>

https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/ <br/>

Se utilizó PowerBI como herramienta visual para presentar de manera gráfica el análisis desarrollado en base al KPI propuesto y los KPIs sugeridos.

**KPIs**
- Evaluar el aumento o disminución de la variación porcentual trimestral del servicio de internet, cada 100 hogares por provincia.
- Evaluar el aumento o disminución de ingresos anuales por la prestación de internet fijo.
- Evaluar el aumento o disminución de la variación porcentual trimestral en el uso de tecnología de conexión a internet fijo.
- Evaluar el estado de las localidades con respecto al tipo de conexión a internet.

---

## Análisis exploratorio de los datos (EDA)

Se utilizó python como herramienta para el EDA, en un documento jupiter notebook: EDA.ipnb que se encuentra en este repositorio.

Datasets analizados:

* Penetración de Internet fijo (accesos por cada 100 hogares)
* Penetración por hogares nacional de Internet fijo
* Total nacional de accesos a Internet fijo por banda ancha y banda angosta
* Accesos a banda ancha y banda angosta por provincia
* Serie trimestral de accesos a Internet fijo por tecnología
* Acceso a Internet fijo por tecnología y provincia
* Velocidad Media de bajada de Internet fijo
* Velocidad media de bajada de Internet fijo por provincia
* Distribución de los accesos totales nacionales a Internet fijo por velocidad
* Acceso a Internet Fijo por rangos de velocidad de bajada y provincia
* Accesos a Internet fijo por velocidad bajada y provincia
* Ingresos trimestrales por la prestación del servicio de Internet fijo
* Accesos a Internet fijo por velocidad de bajada y localidad
* Accesos a Internet fijo por tecnología y localidad
* Listado de localidades con conectividad a internet
* Conectividad al servicio de Internet

Los datasets contienen información general sobre Acceso a Internet de la Argentina desde el primer trimestre del 2014 al segundo trimestre del 2022

Algunos de los datasets están discriminados por provincia

Algunos de los datasets están discriminados por provincia y localidad

---

## Reporte de Análisis

**KPI:** *Evaluar el aumento o disminución de la variación porcentual trimestral del servicio de internet, cada 100 hogares por provincia.*

Según los datos analizados, a nivel general se ha producido un aumento en la variación porcentual de la penetración de internet, accesos por cada 100 hogares.</br>

Capital Federal es la única provincia que tiene valores en *"Accesos por cada 100 hogares"* mayores a 100 durante todos los años, eso implica que en algunos hogares hay más de un tipo de conexión para acceso de internet.

Considerando los datos del primer cuatrimestre del año 2022, que es el más actual del dataset, la provincia con menor Accesos por cada 100 hogares es Formosa (34.96) y la pronvicia con mayor valor es Capital Federal (111.80)

Las pronvicias con menor Accesos por cada 100 hogares son:

* Formosa (34.96)
* Santa Cruz (43.34)
* San Juan (43.55)
* Chaco (44.06)
* Santiago Del Estero (47.17)

Las pronvicias con mayor Accesos por cada 100 hogares son:

* Córdoba (85.76)
* Chubut (88.05)
* La Pampa (91.66)
* Tierra Del Fuego (98.29)
* Capital Federal (111.80)

El 33.33% de las provincias tienen valor de accesos por cada 100 hogares menor a 50, (12 provincias) <br/>

El 66.67% de las provincias tienen valor de accesos por cada 100 hogares mayor a 50, (12 provincias) <br/>

Las provincias de la zona Centro: Buenos Aires, Capital Federal, Córdoba, Ente Ríos y Santa Fe, se encuentran dentro grupo por encina de 50 accesos por cada 100 hogares

Las provincias de la zona Patagónica también se encuentran dentro grupo por encina de 50 accesos por cada 100 hogares, a excepción de Santa Cruz (36,71)

Las provincias de las regiones del NEA, NOA y Cuyo -a excepción de Salta y San Luis- se encuentran por debajo 50 accesos por cada 100 hogares.

Esto demarca una gran diferencia entre las zonas norte y sur del país.

En la mayoría de los casos el crecimiento o disminución trimestral fue de menos de 10%, muy pocos por encima de 10% y algunas situaciones excepcionales con crecimientos por encima de 100%.

---

**KPI:** *Evaluar el aumento o disminución de ingresos anuales por la prestación de internet fijo.*

Es muy notorio el aumento de ingresos en el período analizado, 2014 a 2015.

A nivel trimestral sólo en 2 oportunidades se han registrado disminición porcentual y en valores muy pequeños:
- 2015 Q2: -3,58%
- 2020 Q3: -0,33%

En 4 períodos ha logrado superar un crecimiento del 20%:
- 2015 Q1: 23,44%
- 2019 Q1: 21,46%
- 2020 Q1: 23,90%
- 2022 Q1: 23,59%

Con respecto al crecimiento anual, en la mayoría fue por encima del 40%.

---

**KPI:** *Evaluar el aumento o disminución de la variación porcentual trimestral en el uso de tecnología de conexión a internet fijo.*

Como resultado de la comparación del último trimestre con datos 2022 Q2 y su equivalente al primero 2014 Q2, se evidencia un crecimiento en la tecnología Fibra Óptica de 22.54%

En el análisis de evolución de tiempo con las diferentes tecnologías, se nota claramente que las más utilizadas son ADSL y Cablemodem.

A nivel global se observa que la tecnología Wireless es la que menos variación ha tenido con el paso del tiempo.

ADSL se ha mantenido con valores cercanos al 50% durante los primeros años y luego ha ido disminuyendo desde el año 2017 con mayor intensidad.

La tecnología Cablemodem estuvo siempre en crecimiento, con pendiente más pronunciada desde 2016 y es la tecnología con mayor cantnidad de conexiones del país.

El año 2017 fue punto de intersección entre el crecimiento de la tecnología cablemodem y decrecimiento de la tecnología ADSL.

La Fibra Óptica es la tecnología que más ha crecido en el paso de los años con crecimiento importante desde el año 2019.

La fibra óptica es la tecnología que las empresas que proveen servicio de internet ofrecen como el servicio que asegura más ancho de banda creciente.

---

**KPI:** *Evaluar el estado de las localidades con respecto al tipo de conexión a internet.*

El 19.18% de las localidades no tienen conexión a internet, 827 localidades sobre un total de 4312.

Todas las provincias tienen al menos una localidad sin conexión a internet.

Las provincias como Chaco, Formosa, Corrientes, se encuentran entre las que tienen menos localidades sin conexión, sin embargo se encuentran entre las provincias con menores accesos por cada 100 hogares.

El 19.34% de las localidades tienen sólo conexión movil a internet, 834 localidades.

El 30.64% de las localidades tienen conexión por fibra óptica a internet, 1321 localidades.

El 19.74% de las localidades tienen conexión por cablemodem a internet, 851 localidades.

---

# Conclusiones

Las provincias que pertenecen regiones Centro y Patagonia son las que más se han beneficiado con las tecnologías, acceso y uso de internet.

Las otras regiones, NEA, NOA y Cuyo, están en proceso de crecimiento pero más lento. Coincide también con otros aspectos: económicos, educación y calidad de vida.

Se ha notado un crecimiento de la tecnología Fibra Optica, que es la que las empresas eligen para asegurar un mejor servicio en todos los aspectos, el 30% de las localidades del país tienen la tecnología pero hay otras que aun prevalencen como más usadas, el proceso de cambio va lento, motivos pueden ser varios: promoción y precio por ejemplo.

A partir de la pandemia se ha establecido el teletrabajo como una alternativa obligatoria y se ha quedado como opcional en muchas situaciones, las clases virtuales y consumo de contenido online con calidad demandan mayores prestaciones.

Es importante la apuesta a un crecimiento general del país en prestaciones de telecomunicaciones para que siga creciendo y evolucionando. Debería ser política de Estado mejorar las prestaciones de los sectores más desfavorecidos que se han mencionado a lo largo del informe.