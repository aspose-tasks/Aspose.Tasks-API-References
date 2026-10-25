---
title: "Tsk.FixedCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynak dışı görev masraflarını gösterir"
type: docs
weight: 430
url: /tr/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

Kaynak olmayan görev masraflarını gösterir.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
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


