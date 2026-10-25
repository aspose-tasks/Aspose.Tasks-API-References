---
title: "Prj.NewTasksEffortDriven"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yeni görevlerin çaba odaklı olup olmadığını belirler"
type: docs
weight: 560
url: /tr/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

Yeni görevlerin çaba odaklı olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## Örnekler

Prj.NewTasksEffortDriven özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


