---
title: "Класс YearlyRepetitionBase"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.YearlyRepetitionBase. Представляет базовый шаблон для годовой позиции дня."
type: docs
weight: 3700
url: /ru/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

Представляет базовый шаблон для годовой позиции дня.

```csharp
public abstract class YearlyRepetitionBase
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


