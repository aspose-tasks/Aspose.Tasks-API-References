---
title: "Класс MonthlyRecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.MonthlyRecurrencePattern. Представляет набор параметров, используемых для создания ежемесячной повторяющейся задачи в проекте"
type: docs
weight: 1080
url: /ru/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Представляет набор параметров, используемых для создания ежемесячной повторяющейся задачи в проекте.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Инициализирует новый экземпляр класса `MonthlyRecurrencePattern`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Получает или задает диапазон повторения. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Получает или задает повторяющийся шаблон. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


