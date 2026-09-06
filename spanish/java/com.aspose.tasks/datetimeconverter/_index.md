---
title: "DateTimeConverter"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un convertidor para convertir fechas a cadena en los niveles de escala de tiempo de la vista."
type: docs
weight: 70
url: /es/java/com.aspose.tasks/datetimeconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class DateTimeConverter extends System.MulticastDelegate
```

Representa un convertidor para convertir fechas a cadena en los niveles de escala de tiempo de la vista.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DateTimeConverter()](#DateTimeConverter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [invoke(Date date)](#invoke-java.util.Date-) | Representa un método convertidor para convertir la fecha a cadena en los niveles de escala de tiempo de la vista. |
### DateTimeConverter() {#DateTimeConverter--}
```
public DateTimeConverter()
```


### invoke(Date date) {#invoke-java.util.Date-}
```
public abstract String invoke(Date date)
```


Representa un método convertidor para convertir la fecha a cadena en los niveles de escala de tiempo de la vista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | java.util.Date | la instancia de la clase `java.util.Date` para convertir a cadena. |

**Returns:**
java.lang.String - la representación en cadena de la fecha especificada.
