---
title: "Класс ByYearWeekDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ByYearWeekDayRepetition. Представляет шаблон, основанный на позиции дня недели в месяце"
type: docs
weight: 200
url: /ru/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Представляет шаблон, основанный на позиции дня недели в месяце.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Инициализирует новый экземпляр класса `ByYearWeekDayRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Получает или задает месяц, в котором задача должна повторяться. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Получает или задает позицию дня недели в месяце, в котором задача должна повторяться. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Получает или задает тип дня недели, в который задача должна повторяться. |

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

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


