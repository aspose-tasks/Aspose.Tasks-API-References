---
title: "TaskBaseline.Duration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskBaseline. Получает или задает запланированную длительность задачи, когда базовый план был сохранён."
type: docs
weight: 20
url: /ru/net/aspose.tasks/taskbaseline/duration/
---
## TaskBaseline.Duration property

Получает или задает запланированную продолжительность задачи, когда базовый план был сохранён.

```csharp
public Duration Duration { get; set; }
```

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

* struct [Duration](../../duration/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


