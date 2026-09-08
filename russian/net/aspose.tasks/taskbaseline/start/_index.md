---
title: "TaskBaseline.Start"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskBaseline. Получает или задает запланированную дату начала задачи, когда была сохранена базовая линия"
type: docs
weight: 70
url: /ru/net/aspose.tasks/taskbaseline/start/
---
## TaskBaseline.Start property

Получает или задает запланированную дату начала задачи, когда базовый план был сохранён.

```csharp
public DateTime Start { get; set; }
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

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


