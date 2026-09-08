---
title: "RecurringInterval.MonthlyDayMonthNumber"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RecurringInterval. Возвращает или задает номер месяца ежемесячных линий прогресса"
type: docs
weight: 70
url: /ru/net/aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/
---
## RecurringInterval.MonthlyDayMonthNumber property

Получает или задает номер месяца ежемесячных линий прогресса.

```csharp
public int MonthlyDayMonthNumber { get; set; }
```

## Примеры

Показывает, как работать с повторяющимся интервалом линий прогресса.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// Позволяет читать линию прогресса
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// Позволяет переопределить повторяющийся интервал
var newInterval = new RecurringInterval();

// Устанавливает значение, указывающее, показывать ли месячные линии прогресса по дню.
interval.MonthlyDay = true;
// Устанавливает номер дня для месячных линий прогресса.
interval.MonthlyDayDayNumber = 1;
// Устанавливает номер месяца для месячных линий прогресса.
interval.MonthlyDayMonthNumber = 1;
// Устанавливает значение, указывающее, показывать ли линии прогресса по первому или последнему предопределённому дню.
interval.MonthlyFirstLast = true;
// Устанавливает тип первого или последнего дня для месячных линий прогресса.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// Устанавливает номер месяца для линий прогресса, которые отображаются по первому или последнему предопределённому дню.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


