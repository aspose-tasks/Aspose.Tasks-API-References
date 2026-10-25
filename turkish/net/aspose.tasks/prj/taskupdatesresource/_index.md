---
title: "Prj.TaskUpdatesResource"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Görev güncellemelerinin kaynakları güncelleyip güncellemeyeceğini belirler"
type: docs
weight: 710
url: /tr/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

Görev güncellemelerinin kaynakları güncelleyip güncellemeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## Örnekler

Prj.TaskUpdatesResource özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


