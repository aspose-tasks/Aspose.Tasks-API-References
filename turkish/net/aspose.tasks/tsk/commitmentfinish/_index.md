---
title: "Tsk.CommitmentFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir teslimatın bitiş tarihi.  Okuma yalnızca XML formatı için desteklenir"
type: docs
weight: 170
url: /tr/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

Teslimatın bitiş tarihi. Okuma yalnızca XML formatı için desteklenir.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Örnekler

Tsk.CommitmentFinish özelliğinin nasıl okunup yazıldığını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


