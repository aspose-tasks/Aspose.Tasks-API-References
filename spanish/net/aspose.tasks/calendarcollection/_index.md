---
title: "Clase CalendarCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.CalendarCollection. Representa una colección de objetos Calendar"
type: docs
weight: 240
url: /es/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Representa una colección de objetos [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `CalendarCollection`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Agrega un nuevo calendario base a este objeto CalendarCollection y devuelve el calendario agregado. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Agrega un nuevo calendario con el calendario base especificado a este objeto CalendarCollection y devuelve el calendario agregado. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Devuelve un calendario con el nombre especificado. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Devuelve un calendario con el UID especificado. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Elimina Calendar de la CalendarCollection del proyecto. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Convierte el objeto CalendarCollection en una lista de objetos [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


