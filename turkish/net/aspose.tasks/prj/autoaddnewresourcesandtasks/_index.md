---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yeni kaynakların veya görevlerin bir kaynak veya görev havuzuna otomatik olarak eklenip eklenmeyeceğini belirler"
type: docs
weight: 50
url: /tr/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Yeni kaynakların veya görevlerin bir kaynak veya görev havuzuna otomatik olarak eklenip eklenmeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Örnekler

Prj.AutoAddNewResourcesAndTasks özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


