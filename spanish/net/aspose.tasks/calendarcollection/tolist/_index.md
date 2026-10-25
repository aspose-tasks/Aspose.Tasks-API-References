---
title: "CalendarCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Convierte el objeto CalendarCollection en una lista de objetos Calendar."
type: docs
weight: 70
url: /es/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Convierte el objeto CalendarCollection en una lista de objetos [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Valor devuelto

Lista de objetos [`Calendar`](../../calendar/).

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


