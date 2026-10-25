---
title: "Tsk.Guid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev için oluşturulan benzersiz kimlik kodları"
type: docs
weight: 460
url: /tr/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Bir görev için oluşturulan benzersiz tanımlama kodları.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Örnekler

Tsk.Guid özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


