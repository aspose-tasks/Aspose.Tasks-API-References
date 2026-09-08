---
title: "Класс ByYearDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ByYearDayRepetition. Представляет шаблон, основанный на абсолютной позиции дня в месяце"
type: docs
weight: 190
url: /ru/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Представляет шаблон, основанный на абсолютной позиции дня в месяце.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Инициализирует новый экземпляр класса `ByYearDayRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Получает или задает позицию дня в месяце, в которой задача должна повторяться. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Получает или задает месяц, в котором задача должна повторяться. |

## Примеры

Показывает, как работать с повторениями по дню года при создании новых повторяющихся задач.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


