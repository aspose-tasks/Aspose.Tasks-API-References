---
title: "CalendarCollection.GetByName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Devuelve un calendario con el nombre especificado."
type: docs
weight: 30
url: /es/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Devuelve un calendario con el nombre especificado.

```csharp
public Calendar GetByName(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre de un calendario. |

### Valor devuelto

Si se encuentra, devuelve el calendario con un nombre especificado; de lo contrario, devuelve null.

## Ejemplos

Muestra cómo obtener calendarios por nombre o por id.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Ver también

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


