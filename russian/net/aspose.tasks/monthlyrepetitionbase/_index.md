---
title: "Класс MonthlyRepetitionBase"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.MonthlyRepetitionBase. Представляет базовый шаблон для позиции дня месяца"
type: docs
weight: 1090
url: /ru/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Представляет базовый шаблон для позиции дня месяца.

```csharp
public abstract class MonthlyRepetitionBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество месяцев, представляющее интервал в месяцах между появлениями. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


