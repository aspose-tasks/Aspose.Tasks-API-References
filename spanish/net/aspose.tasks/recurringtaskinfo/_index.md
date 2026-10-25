---
title: "Clase RecurringTaskInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RecurringTaskInfo. Representa los detalles de una tarea recurrente en un proyecto"
type: docs
weight: 1720
url: /es/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Representa los detalles de una tarea recurrente en un proyecto.

```csharp
public class RecurringTaskInfo
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Obtiene o establece un número de repeticiones para el patrón de recurrencia diario. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Obtiene o establece un valor que indica si se deben usar días laborables para el patrón de recurrencia diario. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Obtiene o establece la duración de una ocurrencia de la tarea recurrente. la instancia de la clase [`Duration`](./duration/). |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Obtiene o establece la fecha en que finalizan las ocurrencias. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Obtiene o establece un número de día del patrón de recurrencia mensual. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Obtiene o establece un día del patrón de recurrencia mensual al usar día ordinal. Puede ser uno de los valores de la enumeración DayOfWeek. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Obtiene o establece un número ordinal del patrón de recurrencia mensual. Puede ser uno de los valores de la enumeración [`OrdinalNumber`](../ordinalnumber/). |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Obtiene o establece un número de repeticiones para el patrón de recurrencia mensual al usar día ordinal. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Obtiene o establece un número de repeticiones para el patrón de recurrencia mensual. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Obtiene o establece un valor que indica si se debe usar día ordinal para el patrón de recurrencia mensual. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Obtiene o establece un número de ocurrencias de la tarea recurrente. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Obtiene o establece un patrón de recurrencia de la tarea recurrente. Puede ser uno de los valores de la enumeración [`RecurrencePattern`](./recurrencepattern/). |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Obtiene o establece la fecha en que comienzan las ocurrencias. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Obtiene la tarea principal de esta instancia de la clase `RecurringTaskInfo`. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Obtiene o establece un valor que indica si se debe usar la fecha de finalización o un número de ocurrencias para la tarea recurrente. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Obtiene o establece una colección de días utilizados en el patrón de recurrencia semanal. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Obtiene o establece un número de repeticiones para el patrón de recurrencia semanal. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Obtiene o establece una fecha para el patrón de recurrencia anual. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Obtiene o establece un día de la semana del patrón de recurrencia anual al usar día ordinal. Puede ser uno de los valores de la enumeración DayOfWeek. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Obtiene o establece un mes del patrón de recurrencia anual al usar día ordinal. Puede ser uno de los valores de la enumeración [`Month`](../month/). |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Obtiene o establece un número ordinal del patrón de recurrencia anual. Puede ser uno de los valores de la enumeración [`OrdinalNumber`](../ordinalnumber/). |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Obtiene o establece un valor que indica si se debe usar el día ordinal para el patrón de recurrencia anual. |

## Ejemplos

Muestra cómo leer la información recurrente de tareas.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// leer información recurrente de tareas
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


