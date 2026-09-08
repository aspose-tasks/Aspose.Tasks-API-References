---
title: "Перечисление MonthItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.MonthItemType. Указывает элемент месяца, для которого запланировано исключение повторения."
type: docs
weight: 1050
url: /ru/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Указывает элемент месяца, для которого запланировано исключение повторения.

```csharp
public enum MonthItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает тип месяца: Undefined. |
| Day | `0` | Указывает тип месяца: Day. |
| Weekday | `1` | Указывает тип месяца: Weekday. |
| WeekendDay | `2` | Указывает тип месяца: WeekendDay. |
| Sunday | `3` | Указывает тип месяца: Sunday. |
| Monday | `4` | Указывает тип месяца: Monday. |
| Tuesday | `5` | Указывает тип месяца: Tuesday. |
| Wednesday | `6` | Указывает тип месяца: Wednesday. |
| Thursday | `7` | Указывает тип месяца: Thursday. |
| Friday | `8` | Указывает тип месяца: Friday. |
| Saturday | `9` | Указывает тип месяца: Saturday. |

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


