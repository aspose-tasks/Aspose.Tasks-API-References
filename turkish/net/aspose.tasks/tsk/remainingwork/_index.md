---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevi veya görev setini tamamlamak için hâlâ gereken süre"
type: docs
weight: 990
url: /tr/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Bir görevi veya görev setini tamamlamak için hâlâ gereken süre.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Örnekler

Tsk.RemainingWork özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


