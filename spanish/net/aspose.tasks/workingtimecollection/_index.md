---
title: "Clase WorkingTimeCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WorkingTimeCollection. Representa una colección de objetos WorkingTimeCollection."
type: docs
weight: 3670
url: /es/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Representa una colección de objetos `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `WorkingTimeCollection`. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Agrega una nueva instancia de WorkingTime a esta colección. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Elimina todos los elementos [`WorkingTime`](../workingtime/) de la colección. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Comprueba si el elemento especificado está en la List. Realiza una búsqueda lineal O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | copia el contenido de una colección en un Array, comenzando en un índice particular. |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Elimina la instancia [`WorkingTime`](../workingtime/) de esta colección. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Convierte el objeto WorkingTimeCollection en una lista de objetos [`WorkingTime`](../workingtime/). |

## Ejemplos

Muestra cómo trabajar con la colección de tiempos de trabajo.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// imprime los tiempos de trabajo del sábado.
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// imprime los tiempos de trabajo del domingo.
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Puedes recorrer más a fondo los tiempos de trabajo y mostrarlos.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Ver también

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


