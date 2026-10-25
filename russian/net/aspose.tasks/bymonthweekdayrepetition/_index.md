---
title: "Класс ByMonthWeekDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ByMonthWeekDayRepetition. Представляет шаблон, основанный на позиции дня недели в месяце"
type: docs
weight: 180
url: /ru/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Представляет шаблон, основанный на позиции дня недели в месяце.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Инициализирует новый экземпляр класса `ByMonthWeekDayRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Получает или задает позицию дня недели в месяце, в который задача должна повторяться. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество месяцев, представляющее интервал в месяцах между появлениями. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Получает или задает тип дня недели, в который задача должна повторяться. |

## Примеры

Показывает, как работать с повторениями дней недели по месяцам при создании новых повторяющихся задач.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


