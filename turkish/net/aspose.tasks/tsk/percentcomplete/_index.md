---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin mevcut durumu, tamamlanan görev süresinin yüzdesi olarak ifade edilir"
type: docs
weight: 880
url: /tr/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

Bir görevin mevcut durumu, görevin süresinin tamamlanma yüzdesi olarak ifade edilir.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Örnekler

Görev ilerlemesini, görev yüzde tamamlamasını güncelleyerek nasıl değiştireceğinizi gösterir.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Görevlere erişin ve yüzde tamamlamayı gösterin
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


