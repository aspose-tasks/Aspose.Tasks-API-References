---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin yinelenen görev serisinin bir parçası olup olmadığını belirler."
type: docs
weight: 670
url: /tr/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Bir görevin yinelenen görevler serisinin bir parçası olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Örnekler

Tsk.IsRecurring özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


