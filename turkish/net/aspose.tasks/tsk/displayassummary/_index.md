---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin özet görev olarak görüntülenip görüntülenmeyeceğini belirler. Okuma yalnızca XML formatı için desteklenir."
type: docs
weight: 280
url: /tr/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Görevin özet görev olarak gösterilip gösterilmeyeceğini belirler. Okuma yalnızca XML formatı için desteklenir.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Örnekler

Tsk.DisplayAsSummary özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


