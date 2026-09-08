---
title: "MonthlyRecurrencePattern.Repetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MonthlyRecurrencePattern. Получает или задает шаблон повторяющегося повторения"
type: docs
weight: 20
url: /ru/net/aspose.tasks/monthlyrecurrencepattern/repetition/
---
## MonthlyRecurrencePattern.Repetition property

Получает или задает повторяющийся шаблон.

```csharp
public MonthlyRepetitionBase Repetition { get; set; }
```

## Примеры

Показывает, как работать с повторениями шаблона ежемесячной периодичности при создании повторяющихся задач.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [MonthlyRepetitionBase](../../monthlyrepetitionbase/)
* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


