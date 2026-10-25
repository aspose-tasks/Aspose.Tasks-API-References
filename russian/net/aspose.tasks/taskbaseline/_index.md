---
title: "Класс TaskBaseline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskBaseline. Представляет базовую линию задачи."
type: docs
weight: 2370
url: /ru/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Представляет базовый план задачи.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Инициализирует новый экземпляр класса `TaskBaseline`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Получает или задает уникальный номер записи данных базовой линии. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Получает или задает запланированную стоимость работы, выполненной ресурсом для проекта на текущую дату. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Получает или задает бюджетную стоимость запланированной работы для ресурса. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Получает или задает прогнозируемую стоимость ресурса при сохранении базовой линии. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Получает или задает запланированную продолжительность задачи, когда базовый план был сохранён. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Получает или задает значение, указывающее, была ли оценена базовая продолжительность задачи. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Получает или задает запланированную дату завершения задачи, когда базовый план был сохранён. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Получает или задает фиксированную стоимость задачи, когда базовый план был сохранён. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Получает или задает значение, указывающее, является ли это промежуточным базовым планом. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Получает или задает запланированную дату начала задачи, когда базовый план был сохранён. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Получает или задает экземпляр TimephasedDataCollection для этого объекта. Временные данные, связанные с базовым планом задачи. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Получает или задает работу, назначенную ресурсу при сохранении базовой линии. Объём назначенной работы ресурсу при сохранении базовой линии. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Реализация интерфейса IComparable. Сравнивает этот экземпляр с указанным объектом Baseline. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Реализация интерфейса IComparable. Сравнивает этот экземпляр с указанным объектом Baseline. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту `TaskBaseline`. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Возвращает значение хэш‑кода для экземпляра класса `TaskBaseline`. |

## Примеры

Показывает, как получить доступ к информации о базовом плане.

```csharp
var project = new Project();

// Создание TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Отображение продолжительности базового плана задачи
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// значение, указывающее, является ли это промежуточным базовым планом
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// вывести временные данные базового плана задачи
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### См. также

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


