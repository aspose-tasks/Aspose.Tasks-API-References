---
title: "Структура Duration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Структура Aspose.Tasks.Duration. Представляет длительность в проекте."
type: docs
weight: 470
url: /ru/net/aspose.tasks/duration/
---
## Duration structure

Представляет длительность в проекте.

```csharp
public struct Duration : IEquatable<Duration>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Возвращает значение, указывающее, является ли единица времени прошедшей. Флаг, определяющий, является ли данный экземпляр Duration прошедшим. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Возвращает значение, указывающее, является ли единица времени оценочной. Флаг, определяющий, является ли данный экземпляр Duration оценочным. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Получает экземпляр [`TimeSpan`](./timespan/) этого объекта Duration. Экземпляр TimeSpan этого объекта Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Получает тип единицы времени для этого объекта. Тип единицы времени этого экземпляра Duration. |

## Методы

| Имя | Описание |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Преобразует указанную строку в экземпляр структуры `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Добавляет указанное значение double к этой длительности. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Добавляет указанную длительность к этой длительности. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Преобразует объект Duration в другую длительность с указанными единицами времени. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Возвращает значение хэш‑кода для этого объекта. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Вычитает указанное значение double из этого экземпляра длительности. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Вычитает указанную длительность из этого экземпляра длительности. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Преобразует объект Duration в значение Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Возвращает строковое представление этого экземпляра. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Разбирает строку длительности в формате "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


