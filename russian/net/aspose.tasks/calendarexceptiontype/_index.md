---
title: "Перечисление CalendarExceptionType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.CalendarExceptionType. Указывает тип исключения календаря."
type: docs
weight: 270
url: /ru/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Указывает тип исключения календаря.

```csharp
public enum CalendarExceptionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Daily | `0` | Указывает тип ежедневного исключения. |
| YearlyByDay | `1` | Указывает тип ежегодного исключения по дню месяца. |
| YearlyByPosition | `2` | Указывает тип ежегодного исключения по позиции. |
| MonthlyByDay | `3` | Указывает тип ежемесячного исключения по дню месяца. |
| MonthlyByPosition | `4` | Указывает тип ежемесячного исключения по позиции. |
| Weekly | `5` | Указывает тип еженедельного исключения. |
| ByDayCount | `6` | Указывает тип исключения по количеству дней. |
| ByWeekDayCount | `7` | Указывает тип исключения по количеству дней недели. |
| NoExceptionType | `8` | Указывает тип отсутствия исключения. |

## Примеры

Показывает, как определить исключение календаря по вхождениям.

```csharp
var project = new Project();

// Определить календарь
var calendar = project.Calendars.Add("Calendar1");

// Определите исключение и укажите вхождения
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Добавить исключение в календарь
calendar.Exceptions.Add(exception);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


