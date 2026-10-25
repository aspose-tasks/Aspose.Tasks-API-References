---
title: "Task.Baselines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Görevin temel değer koleksiyonunu alır veya ayarlar"
type: docs
weight: 130
url: /tr/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Görevin temel değerler koleksiyonunu alır veya ayarlar.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Örnekler

Görevin temellerini okuma yöntemini göster.

```csharp
var project = new Project();

// bir temel ayarla
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Görev temel çizgi süresini göster
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Ayrıca Bakınız

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


