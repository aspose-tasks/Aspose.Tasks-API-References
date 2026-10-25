---
title: "CalendarCollection.GetByUid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Devuelve un calendario con el UID especificado"
type: docs
weight: 40
url: /es/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Devuelve un calendario con el UID especificado.

```csharp
public Calendar GetByUid(int uid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | Int32 | UID de un calendario. |

### Valor devuelto

Calendario con un UID especificado.

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


