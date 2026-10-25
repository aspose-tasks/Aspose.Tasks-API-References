---
title: "CalendarCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Devuelve un enumerador para esta colección."
type: docs
weight: 50
url: /es/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Devuelve un enumerador para esta colección.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Valor devuelto

un enumerador para esta colección.

## Ejemplos

Muestra cómo agregar nuevos calendarios.

```csharp
var project = new Project();

// Se pueden agregar nuevos calendarios a la colección de calendarios de un proyecto usando las sobrecargas del método Add de la colección.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ver también

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


