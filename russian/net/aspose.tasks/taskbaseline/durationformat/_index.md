---
title: "DurationFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает формат отображения длительности базового плана задачи."
type: docs
weight: 30
url: /ru/net/aspose.tasks/taskbaseline/durationformat/
---
## TaskBaseline.DurationFormat property

Получает или задает формат отображения длительности базового плана задачи.

```csharp
public TimeUnitType DurationFormat { get; set; }
```

### Примеры

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
Console.WriteLine("Baseline duration format: {0}", baseline.DurationFormat);
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

* enum [TimeUnitType](../../timeunittype)
* class [TaskBaseline](../../taskbaseline)
* namespace [Aspose.Tasks](../../taskbaseline)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
