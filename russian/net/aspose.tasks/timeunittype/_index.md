---
title: "Перечисление TimeUnitType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.TimeUnitType. Указывает тип единицы времени"
type: docs
weight: 2570
url: /ru/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Указывает тип единицы времени.

```csharp
public enum TimeUnitType : sbyte
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает, что значение Undefined означает, что поле не было определено в оригинальном файле проекта. |
| Minute | `0` | Указывает тип единицы времени Минут. |
| ElapsedMinute | `1` | Указывает тип единицы времени прошедших минут. |
| Hour | `2` | Указывает тип единицы времени Час. |
| ElapsedHour | `3` | Указывает тип единицы времени прошедших часов. |
| Day | `4` | Указывает тип единицы времени День. |
| ElapsedDay | `5` | Указывает тип единицы времени прошедших дней. |
| Week | `6` | Указывает тип единицы времени Неделя. |
| ElapsedWeek | `7` | Указывает тип единицы времени прошедших недель. |
| Month | `8` | Указывает тип единицы времени Месяц. |
| ElapsedMonth | `9` | Указывает тип единицы времени прошедших месяцев. |
| Percent | `10` | Указывает тип единицы времени Процент. |
| ElapsedPercent | `11` | Указывает тип единицы времени прошедших процентов. |
| Null | `12` | Указывает тип единицы времени Null. |
| MinuteEstimated | `13` | Указывает тип единицы времени оценки Минут. |
| ElapsedMinuteEstimated | `14` | Указывает тип единицы времени оценки прошедших минут. |
| HourEstimated | `15` | Указывает тип единицы времени оценки Час. |
| ElapsedHourEstimated | `16` | Указывает тип единицы времени оценки прошедших часов. |
| DayEstimated | `17` | Указывает тип единицы времени оценки День. |
| ElapsedDayEstimated | `18` | Указывает тип единицы времени оценки прошедших дней. |
| WeekEstimated | `19` | Указывает тип единицы времени оценки Неделя. |
| ElapsedWeekEstimated | `20` | Указывает тип единицы времени оценки прошедших недель. |
| MonthEstimated | `21` | Указывает тип единицы времени оценки Месяц. |
| ElapsedMonthEstimated | `22` | Указывает тип единицы времени оценки прошедших месяцев. |
| PercentEstimated | `23` | Указывает тип единицы времени оценки Процент. |
| ElapsedPercentEstimated | `24` | Указывает тип единицы времени, оцениваемый в процентах прошедшего времени. |
| Year | `25` | Указывает тип единицы времени — год. |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как преобразовать длительность в различные типы единиц времени.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Получить задачу для расчёта её длительности в разных форматах
var task = project.RootTask.Children.GetById(1);

// Получить длительность в минутах, днях, часах, неделях и месяцах
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


