---
title: "Duration.ToDouble"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Преобразует объект Duration в значение Double."
type: docs
weight: 110
url: /ru/net/aspose.tasks/duration/todouble/
---
## Duration.ToDouble method

Преобразует объект Duration в значение Double.

```csharp
public double ToDouble()
```

### Возвращаемое значение

Преобразованное значение.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


