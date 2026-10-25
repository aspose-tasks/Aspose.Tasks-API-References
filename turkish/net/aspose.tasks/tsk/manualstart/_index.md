---
title: "Tsk.ManualStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin manuel olarak planlanan başlangıcını tanımlar"
type: docs
weight: 800
url: /tr/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Bir görevin manuel olarak planlanan başlangıcını tanımlar.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Örnekler

Tsk.ManualStart özelliğinin nasıl okunup yazıldığını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


