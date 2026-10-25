---
title: "RecurringTaskInfo.YearlyOrdinalDay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad RecurringTaskInfo. Obtiene o establece un día de la semana del patrón de recurrencia anual al usar el día ordinal. Puede ser uno de los valores de la enumeración DayOfWeek"
type: docs
weight: 190
url: /es/net/aspose.tasks/recurringtaskinfo/yearlyordinalday/
---
## RecurringTaskInfo.YearlyOrdinalDay property

Obtiene o establece un día de la semana del patrón de recurrencia anual al usar día ordinal. Puede ser uno de los valores de la enumeración DayOfWeek.

```csharp
public DayOfWeek YearlyOrdinalDay { get; set; }
```

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

* class [RecurringTaskInfo](../)
* namespace [Aspose.Tasks](../../recurringtaskinfo/)
* assembly [Aspose.Tasks](../../../)


