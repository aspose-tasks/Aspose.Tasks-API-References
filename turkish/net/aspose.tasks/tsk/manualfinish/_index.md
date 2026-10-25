---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin manuel olarak planlanan bitişini tanımlar"
type: docs
weight: 790
url: /tr/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Bir görevin manuel olarak planlanan bitişini tanımlar.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Örnekler

Tsk.ManualFinish özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


