---
title: "Duration.Subtract"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Вычитает указанную длительность из этого экземпляра Duration."
type: docs
weight: 100
url: /ru/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Вычитает указанную длительность из этого экземпляра длительности.

```csharp
public Duration Subtract(Duration d)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| d | Duration | указанный экземпляр [`Duration`](../), из которого вычитается из текущего экземпляра. |

### Возвращаемое значение

Новый объект длительности, представляющий значение этого экземпляра минус указанное значение длительности.

## Примеры

Показывает, как изменить длительность задач.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// получить задачу
var task1 = project.RootTask.Children.GetById(1);

// обновить длительность задачи
var duration1 = task1.Get(Tsk.Duration);

// вычесть один день из задачи 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// установить новую длительность для задачи
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// получить другую задачу
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// изменить длительность, используя фактический тип единицы времени
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// установить новую длительность для задачи
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Вычитает указанное значение double из этого экземпляра длительности.

```csharp
public Duration Subtract(double val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | Double | указанное значение Double для вычитания из этого экземпляра. |

### Возвращаемое значение

Новый объект длительности, представляющий значение этого экземпляра минус указанное значение длительности.

## Примеры

Показывает, как изменить длительность задач.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// получить задачу
var task1 = project.RootTask.Children.GetById(1);

// обновить длительность задачи
var duration1 = task1.Get(Tsk.Duration);

// вычесть один день из задачи 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// установить новую длительность для задачи
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// получить другую задачу
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// изменить длительность, используя фактический тип единицы времени
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// установить новую длительность для задачи
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


