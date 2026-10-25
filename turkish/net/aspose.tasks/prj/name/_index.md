---
title: "Prj.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Projenin adı"
type: docs
weight: 540
url: /tr/net/aspose.tasks/prj/name/
---
## Prj.Name field

Projenin adı.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Örnekler

Proje adının nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


