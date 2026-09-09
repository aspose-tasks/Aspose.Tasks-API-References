---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin mevcut durumu, tamamlanan işin yüzdesi olarak ifade edilir"
type: docs
weight: 890
url: /tr/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

Bir görevin mevcut durumu, tamamlanan iş yüzdesi olarak ifade edilir.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Örnekler

Tsk.PercentWorkComplete özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


