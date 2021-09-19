# Cadena Internacional de Supermercados

Un supermercado internacional con cientos de centros repartidos por 23 países desea una gestión de tickets. 

Un ticket consta de:

* Cabecera: con distintos campos dependiendo del país pero siempre el nombre el nombre de la cadena y la fecha y hora 
de comienzo del ticket de compra
* Cuerpo:  Una secuencia de líneas que se expondrán posteriormente
* Pie: con distintos campos dependiendo del país pero siempre el nombre el nombre de la cadena y la fecha y hora de 
comienzo del ticket de compra

Una línea puede ser:

* De venta, que refleja el código, descripción, unidades y 
precio
* De repetición, que refleja otra línea exactamente igual a la 
dada por el número de la secuencia de líneas
* De anulación, que refleja el número de línea anterior 
anulada con un saldo negativo igual a la línea que anula
* De devolución, que refleja el código
* …
* Dependiendo del país existirán unos tipos de líneas u otros 
aunque venta, repetición y anulación estás presentes en 
todos. Y, por ejemplo, en España existen devoluciones pero 
en Francia no



