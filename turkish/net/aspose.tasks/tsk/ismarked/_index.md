---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin daha fazla işlem için işaretlenip işaretlenmediğini veya bir tür tanımlama yapılıp yapılmadığını gösterir."
type: docs
weight: 620
url: /tr/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Bir görevin daha fazla eylem için işaretlenip işaretlenmediğini veya bir tür tanımlama yapılıp yapılmadığını gösterir.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Açıklamalar

Yalnızca mpp dosya formatı için geçerlidir.

## Örnekler

Tsk.IsMarked özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


