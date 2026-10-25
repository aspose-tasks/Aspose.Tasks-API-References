---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin manuel olarak planlanan süresini tanımlar"
type: docs
weight: 780
url: /tr/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Bir görevin manuel olarak planlanan süresini tanımlar.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Örnekler

Tsk.ManualDuration özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


