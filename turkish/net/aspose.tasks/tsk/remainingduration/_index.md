---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin tamamlanmamış kısmını tamamlamak için gereken süre"
type: docs
weight: 960
url: /tr/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Bir görevin tamamlanmamış kısmını tamamlamak için gereken süre.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Örnekler

Tsk.RemainingDuration özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


