---
title: "Prj.AdminProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin idari proje olup olmadığını belirler"
type: docs
weight: 20
url: /tr/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

Bir projenin idari proje olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## Örnekler

Prj.AdminProject özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


