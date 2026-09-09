---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev için kalan planlanmış fazla mesai gideri."
type: docs
weight: 970
url: /tr/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

Bir görev için kalan planlanmış fazla mesai gideri.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Örnekler

Tsk.RemainingOvertimeCost özelliğinin nasıl okunup yazıldığını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


