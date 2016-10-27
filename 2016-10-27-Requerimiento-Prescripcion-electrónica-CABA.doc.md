---
title: Requerimiento Prescripcion electrónica CABA.doc
layout: post
author: ciannicello
permalink: /requerimiento-prescripcion-electrónica-caba.doc/
source-id: 11WdadBYtmmr3nrRksCYHq5yC3rs0Dr17SJGY1hbJ9Qs
published: true
---
![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_0.png)

**Requerimiento de Desarrollo**

**Historia Clinica Electrónica**

**Prescripciones Médicas Farmacológicas**

**_Dirección de Informática Clínica, Estadística y Epidemiológica_**

**_Sub Secretaría de Planificación Sanitaria_**

**_Ministerio de Salud_**

1. **Contexto:**

El módulo de Prescripciones médicas, que están dentro de la Historia Clinica Electrónica (HCE), en la cual se utilizara para realizar prescripciones médicas farmacológicas, el mismo teniendo integración con Terminología, que tendrá interacción con el módulo de Farmacia para la dispensación del fármaco prescrito.

2. **Descripción del requerimiento:**

A continuación se detallara el requerimiento descrito para la prescripción farmacológicas propiamente dicha.

Contará con un buscador único. En el cual será el servicio de respuesta terminología, en el cual en este caso se puede buscar el nombre del fármaco ya sea por nombre comercial y/o genérico. Como se observa en la imagen 1.

![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_1.png)

Imagen 1. Buscador de medicamentos.

Al introducir la palabras con un mínimo de 3 caracteres, realizara la búsqueda del fármaco, como se observa en la imagen 2.

![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_2.png)

Imagen 2. Busqueda de fármaco

Como se visualiza en la Imagen 2, los datos a ser mostrados son los fármacos asociados al fármaco buscado, visualizandose con las diferentes presentaciones que tiene el fármaco los mismo con link de acceso.

En la parte superior se observa la cantidad de resultados y el tiempo de duración de la busqueda seleccionada.

En caso de selección de un fármaco en este caso de ejemplo: "Lorazepma 1mg comprimido" mostrara la pantalla de la precarga de las indicaciones fármacologicas. Ver imagen 3.

![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_3.png)

Imagen 3. Prescripcipones fármacologicas.

Describiremos la imagen 3.

Continua para realizar la busqueda:

Se observa el Fármaco seleccionado en negrita: "**Lorazepam 1mg comprimido", **con link de acceso de “Vademecum”, para consultar el vademecum, del fármaco seleccionado.

* **_Dosis (*): _**La dosis viene precargada del fármaco seleccionado, la misma debe ser editable, de carácter númerico y con 3 decimales.

* **_Unidad de medida (*): _**La unidad de medida vendrá precargada del fármaco seleccionado, la misma no podrá ser editable.

* **_Vía de Aministracción (*): _**La vía de administracción debe venir precargada, la misma puede ser editable, con combo box predefinido de la tabla de Vía de Administración.

* **_Frecuencia (*): _**La frecuencia, será un combo box la misma que es definida de la tabla de Frecuencia.

* **_Tipo de tratamiento (*): _*** *El tipo de tratamiento será tipo button bar, la que podrá ser seleccionada con dos opciones como aguda o crónica.

* **_Fecha de Inicio (*): _**Carga de fecha en modo dd/mm/aaaa o con selección por fecha mediante calendario, la misma no podrá ser previa al dia de la prescripción. Por defecto trae la fecha del día.

* **_Fecha de Finalización (*): _**Carga de fecha en modo dd/mm/aaaa o con selección por fecha mediante calendario, la misma debe ser mayor a la fecha actual de prescripción..

* **_Cantidad Total: _**Cantidad total se muestra en dos campos, la misma no es editable, es la resultante del cálculo de la cantidad de días de fechas inicio y fecha de finalización con el multiplicador la frecuencia seleccionada por el médico, y de acuerdo a la dosis de la prescripción.

**Ejemplo: **Si se realiza la fecha de inicio 01/09/2016 y la fecha de finalización 10/09/2016, siendo la misma por 10 días. Siendo seleccionada en este ejemplo la frecuenciua de cada 12 horas, siendo que tiene que recibir 2 por día, se multiplicada 10 x 2 = 20 x 1 =20. En este caso la dosis fue de 1 mg.

En caso que la dosis fuese de 2mg, realozando la cuenta previa mostrara 40 comprimidos a dispensarse.

Posterior a ello se mostrara la forma farmaceutica en la que debe ser dispensada.

* **_Stock de Farmacia:_**** **El stock de farmacia, muestra de acuerdo al logueo de la CESAC que el profesional se logueo, mostrara los productos disponibles en esa farmacia. En la captura se visualiza la cantidad de fármacos que existe en la CESAC 5.

* **_Asociar problemas: _**En la parte inferior tal cual como se visualiza la imagen 3, se observa en el lado izquierdo, los problemas que ya tiene asociados  el paciente, desde la solapa de nueva consulta. La misma que podra ser elegible para poder asociar a la prescripción farmacólogica, la misma no es de obligatoria, para continuar la prescripción.

Se incluye al igual que en la evoluciones un buscador de problemas para poder agregar un problema al paciente para asociarlo a la prescripción médicas.

* **_Botones:_**

    * **_Aceptar: _** Al seleccionar este botón efectivizara la prescripción cargada.

    * **_Cancelar: _*** *La misma no generara una acción, de la precarga.

* Los campos descritos con asterisco deben ser obligatorios para la carga asi poder generar la prescripción fármacologica.

En el lado izquierdo mostrara el Historial de prescripciones activas del paciente: como se observa en la imagen 4.

![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_4.png)

Imagen 4. Prescripciones fármacologicas.

Las prescripciones fármacologicas:

Se observa la fecha y hora de la prescripción:  formato dd/mm/aaaa y hh:mm formato de 24 horas.

y a lado las siguientes filas:

* Nombre del fármaco seleccionado. Dosis precaragada por el profesional:

* Vía de administración: Seleccionada por el profesiona; Frecuencia del fármaco.l

* Fecha de Inicio y Fin

* Prescrito por: Muestra el nombre del profesiona con el número de matricula nacional.

* Problema: Muestra el problema asociado a la prescripción seleccionada por el profesional.

* Se observa en la imagen ![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_5.png)la misma que realiza para realizar la edición de dicho prescripción, cuando se realice el clic en la iconografia,mostrara la precarga realizada para este fármaco tal como se visualiza en la imagen 3. En la cual el profesional podra actualizar la prescricpción fármacologica.

**_Historial de prescripciones: _** Tal cual como se muestra en las prescripciones, activas, se solicita agregar una solapa para visualizar el historal de prescripciones del paciente ordenadas por meses en este ejemplo se observam las del último mes.

![image alt text]({{ site.url }}/public/9TdNHgbg7H075a6Tl1KeSA_img_6.png)

Imagen 5. Historial de Prescripciones

El orden de la visualización de los campos es el mismo que se detallo previamente. 

3. **s**

