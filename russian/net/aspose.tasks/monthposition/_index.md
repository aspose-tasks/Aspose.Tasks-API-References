---
title: "Перечисление MonthPosition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.MonthPosition. Указывает позицию элемента месяца внутри месяца."
type: docs
weight: 1070
url: /ru/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Указывает позицию элемента месяца внутри месяца.

```csharp
public enum MonthPosition
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает неопределённую позицию месяца. |
| First | `0` | Указывает позицию месяца — первая. |
| Second | `1` | Указывает позицию месяца — вторая. |
| Third | `2` | Указывает позицию месяца — третья. |
| Fourth | `3` | Указывает позицию месяца в четвертом положении. |
| Last | `4` | Указывает позицию месяца в последнем положении. |

## Примеры

Показывает, как определить исключение календаря по дню месяца.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// создать календарь
var calendar = project.Calendars.Add("Calendar1");

// создать исключение календаря для каждой пятницы
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// проверьте, что пятница является исключительной
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// добавьте исключение в календарь
calendar.Exceptions.Add(exception);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


