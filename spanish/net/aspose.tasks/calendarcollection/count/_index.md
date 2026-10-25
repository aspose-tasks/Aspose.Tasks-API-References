---
title: "CalendarCollection.Count"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad CalendarCollection. Obtiene el número de objetos contenidos en este objeto CalendarCollection"
type: docs
weight: 10
url: /es/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Obtiene el número de objetos contenidos en este objeto [`CalendarCollection`](../).

```csharp
public int Count { get; }
```

## Ejemplos

Muestra cómo iterar sobre la colección de calendarios.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ver también

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


