---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin manuel olarak planlanıp planlanmadığını belirler"
type: docs
weight: 610
url: /tr/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Bir görevin elle zamanlanıp zamanlanmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Örnekler

Tsk.IsManual özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


