---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ByYearDayRepetition. Инициализирует новый экземпляр класса ByYearDayRepetition"
type: docs
weight: 10
url: /ru/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

Инициализирует новый экземпляр класса [`ByYearDayRepetition`](../).

```csharp
public ByYearDayRepetition()
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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


