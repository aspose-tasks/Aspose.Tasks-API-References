---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. GanttChart görünümünde bir özet görevin genişletilip genişletilmediğini belirler."
type: docs
weight: 590
url: /tr/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Özet görevin GanttChart görünümünde genişletilip genişletilmediğini belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Örnekler

Tsk.IsExpanded özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


