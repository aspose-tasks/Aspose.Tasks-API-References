---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Atanan kaynaklar tarafından görevlerde zaten yapılan fazla mesai çalışması için oluşan maliyetler."
type: docs
weight: 50
url: /tr/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Atanan kaynaklar tarafından görevlerde zaten yapılan fazla mesai çalışması için oluşan maliyetler.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Örnekler

Tsk.ActualOvertimeCost özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


