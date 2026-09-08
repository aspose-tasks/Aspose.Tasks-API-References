---
title: "Перечисление Month"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Month. Указывает месяц."
type: docs
weight: 1040
url: /ru/net/aspose.tasks/month/
---
## Month enumeration

Указывает месяц.

```csharp
public enum Month
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает, что значение не было определено в оригинальном файле проекта. |
| January | `0` | Указывает месяц январь. |
| February | `1` | Указывает месяц февраль. |
| March | `2` | Указывает месяц март. |
| April | `3` | Указывает месяц апрель. |
| May | `4` | Указывает месяц май. |
| June | `5` | Указывает месяц июнь. |
| July | `6` | Указывает месяц июль. |
| August | `7` | Указывает месяц август. |
| September | `8` | Указывает месяц сентябрь. |
| October | `9` | Указывает месяц октябрь. |
| November | `10` | Указывает месяц ноябрь. |
| December | `11` | Указывает месяц декабрь. |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

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


