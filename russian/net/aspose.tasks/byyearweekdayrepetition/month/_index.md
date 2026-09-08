---
title: "ByYearWeekDayRepetition.Month"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ByYearWeekDayRepetition. Возвращает или задает месяц, в который задача должна повторяться"
type: docs
weight: 20
url: /ru/net/aspose.tasks/byyearweekdayrepetition/month/
---
## ByYearWeekDayRepetition.Month property

Получает или задает месяц, в котором задача должна повторяться.

```csharp
public Month Month { get; set; }
```

## Примеры

Показывает, как работать с повторениями по дням недели в году при создании новых повторяющихся задач.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### См. также

* enum [Month](../../month/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


