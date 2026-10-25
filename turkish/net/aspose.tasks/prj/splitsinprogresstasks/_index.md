---
title: "Prj.SplitsInProgressTasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Devam eden görevlerin bölünebilir olup olmadığını belirler"
type: docs
weight: 650
url: /tr/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Devam eden görevlerin bölünebilir olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Örnekler

Prj.SplitsInProgressTasks özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


