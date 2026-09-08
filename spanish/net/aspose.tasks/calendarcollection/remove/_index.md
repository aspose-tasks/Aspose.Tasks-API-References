---
title: "CalendarCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Elimina el calendario de la CalendarCollection del proyecto."
type: docs
weight: 60
url: /es/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Elimina Calendar de la CalendarCollection del proyecto.

```csharp
public bool Remove(Calendar item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | Calendar | El calendario a eliminar. |

### Valor devuelto

Si se elimina devuelve true, de lo contrario devuelve false.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Se lanza cuando no se puede eliminar el calendario. |

## Ejemplos

Muestra cómo reemplazar un calendario en la colección.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// agregar nuevo calendario
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


