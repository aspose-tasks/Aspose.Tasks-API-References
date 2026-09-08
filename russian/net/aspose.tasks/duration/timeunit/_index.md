---
title: "Duration.TimeUnit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Duration. Получает тип единицы времени для этого объекта. Тип единицы времени этого экземпляра Duration."
type: docs
weight: 50
url: /ru/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Получает тип единицы времени для этого объекта. Тип единицы времени этого экземпляра Duration.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Примеры

Показывает, как обновить длительность задач.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// получить задачу
var task1 = project.RootTask.Children.GetById(1);

// обновить длительность задачи
var duration1 = task1.Get(Tsk.Duration);

// добавить один день к задаче 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// установить новую длительность для задачи
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// получить другую задачу
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// изменить длительность, используя фактический тип единицы времени
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// установить новую длительность для задачи
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### См. также

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


