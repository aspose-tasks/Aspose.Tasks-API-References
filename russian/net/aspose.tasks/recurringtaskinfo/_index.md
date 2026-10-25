---
title: "Класс RecurringTaskInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.RecurringTaskInfo класс. Представляет детали повторяющейся задачи в проекте."
type: docs
weight: 1720
url: /ru/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Представляет детали повторяющейся задачи в проекте.

```csharp
public class RecurringTaskInfo
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Получает или задает количество повторений для ежедневного шаблона повторения. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Получает или задает значение, указывающее, использовать ли рабочие дни для ежедневного шаблона повторения. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Получает или задает продолжительность одного появления повторяющейся задачи. экземпляр класса [`Duration`](./duration/). |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Получает или задает дату завершения появлений. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Получает или задает количество дней в месячном шаблоне повторения. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Получает или задает день месячного шаблона повторения при использовании порядкового дня. Может быть одним из значений перечисления DayOfWeek. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Получает или задает порядковый номер месячного шаблона повторения. Может быть одним из значений перечисления [`OrdinalNumber`](../ordinalnumber/). |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Получает или задает количество повторений для месячного шаблона повторения при использовании порядкового дня. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Получает или задает количество повторений для месячного шаблона повторения. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Получает или задает значение, указывающее, использовать ли порядковый день для месячного шаблона повторения. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Получает или задает количество появлений повторяющейся задачи. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Получает или задает шаблон повторения повторяющейся задачи. Может быть одним из значений перечисления [`RecurrencePattern`](./recurrencepattern/). |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Получает или задает дату начала появлений. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Получает родительскую задачу данного экземпляра класса `RecurringTaskInfo`. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Получает или задает значение, указывающее, использовать ли конечную дату или количество повторений для повторяющейся задачи. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Получает или задает коллекцию дней, используемых в недельном шаблоне повторения. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Получает или задает количество повторений для недельного шаблона повторения. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Получает или задает дату для годового шаблона повторения. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Получает или задает день недели годового шаблона повторения при использовании порядкового дня. Может принимать одно из значений перечисления DayOfWeek. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Получает или задает месяц годового шаблона повторения при использовании порядкового дня. Может принимать одно из значений перечисления [`Month`](../month/). |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Получает или задает порядковый номер годового шаблона повторения. Может принимать одно из значений перечисления [`OrdinalNumber`](../ordinalnumber/). |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Получает или задает значение, указывающее, использовать ли порядковый день для годового шаблона повторения. |

## Примеры

Показывает, как читать информацию о повторяющихся задачах.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// читать информацию о повторяющихся задачах
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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


