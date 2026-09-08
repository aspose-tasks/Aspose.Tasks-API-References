---
title: "Класс ByMonthDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ByMonthDayRepetition. Представляет шаблон, основанный на абсолютной позиции дня в месяце."
type: docs
weight: 170
url: /ru/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Представляет шаблон, основанный на абсолютной позиции дня в месяце.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Инициализирует новый экземпляр класса `ByMonthDayRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Получает или задает позицию дня в месяце, в которую задача должна повторяться. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество месяцев, представляющее интервал в месяцах между появлениями. |

## Примеры

Показывает, как работать с повторениями по дням месяца при создании новых повторяющихся задач.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


