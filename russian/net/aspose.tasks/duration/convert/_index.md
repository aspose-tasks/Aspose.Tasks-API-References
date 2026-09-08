---
title: "Duration.Convert"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Преобразует объект Duration в другую длительность с указанными единицами времени."
type: docs
weight: 70
url: /ru/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Преобразует объект Duration в другую длительность с указанными единицами времени.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| timeUnitType | TimeUnitType | указанный тип единицы времени. |

### Возвращаемое значение

возвращает новую длительность с указанным типом единицы.

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

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


