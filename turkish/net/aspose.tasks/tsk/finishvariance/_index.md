---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev veya atamanın temel bitiş tarihi ile mevcut bitiş tarihi arasındaki farkı temsil eden zaman"
type: docs
weight: 420
url: /tr/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Bir görev veya atamanın temel bitiş tarihi ile mevcut bitiş tarihi arasındaki farkı temsil eden zaman.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Örnekler

Tsk.FinishVariance özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


