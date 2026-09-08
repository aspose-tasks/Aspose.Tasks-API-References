---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MonthlyRepetitionBase. Возвращает или задает количество месяцев, представляющее интервал в месяцах между повторениями."
type: docs
weight: 10
url: /ru/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

Получает или задает количество месяцев, представляющее интервал в месяцах между появлениями.

```csharp
public int RepetitionInterval { get; set; }
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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


