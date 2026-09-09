---
title: "Tsk.IsSubproject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin eklenmiş bir proje olup olmadığını belirler"
type: docs
weight: 700
url: /tr/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Bir görevin eklenmiş bir proje olup olmadığını belirler.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Örnekler

Tsk.IsSubproject özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


