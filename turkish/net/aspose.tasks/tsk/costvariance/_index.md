---
title: "Tsk.CostVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev kaynağı veya ataması için temel maliyet ile toplam maliyet arasındaki fark."
type: docs
weight: 240
url: /tr/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

Bir görev, kaynak veya atama için temel maliyet ile toplam maliyet arasındaki fark.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
```

## Örnekler

Görev maliyetlerini okuma yöntemini gösterir.

```csharp
var project = new Project();

// Görev ekle ve maliyeti ayarla
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Görevin maliyetle ilgili özelliklerini göster
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


