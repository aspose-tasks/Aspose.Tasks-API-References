---
title: "Tsk.Cost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevlere atanan kaynaklar tarafından gerçekleştirilen iş için zaten oluşmuş maliyetler ve kalan iş için planlanan maliyetler dahil olmak üzere, bir görev için toplam planlanan veya öngörülen maliyeti gösterir"
type: docs
weight: 230
url: /tr/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

Görevlere atanan kaynaklar tarafından yapılan iş için zaten oluşmuş maliyetler ve kalan iş için planlanan maliyetler temel alınarak bir görev için toplam planlanan veya öngörülen maliyet.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


