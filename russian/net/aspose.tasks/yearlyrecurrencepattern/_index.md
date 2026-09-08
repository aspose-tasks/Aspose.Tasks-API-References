---
title: "Класс YearlyRecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.YearlyRecurrencePattern. Представляет набор параметров, используемых для создания ежегодно повторяющейся задачи в проекте"
type: docs
weight: 3690
url: /ru/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Представляет набор параметров, используемых для создания ежегодной повторяющейся задачи в проекте.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Инициализирует новый экземпляр класса `YearlyRecurrencePattern`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Получает или задает диапазон повторения. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Получает или задает шаблон позиции повторения. |

## Примеры

Показывает, как работать с ежегодными шаблонами повторения при создании повторяющихся задач.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


