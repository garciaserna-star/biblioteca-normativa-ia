# Actualizar la interfaz de la biblioteca

Copia este encargo en el chat cuando cambien el índice, las fichas o los informes de novedades.

```text
Actualiza biblioteca.html en esta carpeta y conserva su diseño y sus funciones.
Lee la hoja biblioteca de biblioteca.xlsx y usa una fila por ID. Para cada fila
lee la ficha Markdown indicada por la columna ficha. No alteres el Excel, las
fichas, los informes ni los documentos de la biblioteca.

Sustituye el JSON del elemento script con id biblioteca-datos. Mantén las claves
updated, columns, documents y stateChanges. Usa la fecha de hoy en updated,
columnas del índice en columns y un objeto por documento en documents. Conserva
todos los valores del índice y representa las fechas como AAAA-MM-DD. Mantén
PENDIENTE cuando la fuente lo indique. Añade fichaMarkdown con el texto íntegro,
fichaTitulo con el título, fichaCampos con pares de etiqueta y valor,
fichaSecciones con objetos {title, lines} y fechasClave con objetos {fecha,texto}
a partir de las fechas completas que consten en la sección Fechas clave.
Si falta una ficha, indica el ID en el resultado y deja sus datos de ficha vacíos.

Incluye las altas de las últimas cuatro semanas a partir de fecha_alta, usando
la fecha de actualización como cierre del período. Lee novedades/*.md y registra
como stateChanges solo transiciones verificadas de entradas del índice. Usa
{fecha,id,anterior,nuevo,url} por cambio y omite propuestas, recordatorios y
estados sin confirmar. Una línea inequívoca en la sección Cambios de estado
puede seguir el formato «- AAAA-MM-DD | ID | estado anterior | estado nuevo | URL».
Si los informes usan prosa, extrae solo cambios explícitos con evidencia. No
deduzcas un cambio a partir del estado actual.

Escapa cada carácter < del JSON como \u003c antes de incrustarlo. Mantén
biblioteca.html como un único archivo que se abre con doble clic, sin servidor,
fuentes remotas ni librerías externas. Verifica el número de documentos, los cinco
filtros, la búsqueda, la ficha completa, la línea de tiempo y que el CSV contiene
solo las filas visibles. Informa de cualquier dato o ficha que no pudiste leer.
```
