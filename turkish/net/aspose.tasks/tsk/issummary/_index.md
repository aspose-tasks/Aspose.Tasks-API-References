---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin özet görev olup olmadığını belirler"
type: docs
weight: 720
url: /tr/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Bir görevin özet görev olup olmadığını belirler.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Örnekler

Tsk.IsSummary özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


