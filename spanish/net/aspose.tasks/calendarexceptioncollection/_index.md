---
title: "Clase CalendarExceptionCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.CalendarExceptionCollection clase. Representa una colección de objetos CalendarException"
type: docs
weight: 260
url: /es/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Representa una colección de [`CalendarException`](../calendarexception/) objetos.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `CalendarExceptionCollection`. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Obtiene el calendario principal para este objeto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Agrega una instancia de CalendarException a este objeto de colección. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Agrega un rango de excepciones a la lista interna. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Elimina todos los elementos del `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Elimina la instancia [`CalendarException`](../calendarexception/) de esta colección. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Convierte el objeto CalendarExceptionCollection a una lista de objetos [`CalendarException`](../calendarexception/). |

## Ejemplos

Muestra cómo usar la colección de excepciones de calendario para definir excepciones de calendario.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// eliminar todas las excepciones
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Ver también

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


