---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir alt projenin yalnızca okunur olup olmadığını belirler."
type: docs
weight: 710
url: /tr/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

Bir alt projenin yalnızca okunur olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## Örnekler

Tsk.IsSubprojectReadOnly özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


