---
title: "Prj.ProjectExternallyEdited"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Projenin dışarıdan düzenlenip düzenlenmediğini belirler"
type: docs
weight: 590
url: /tr/net/aspose.tasks/prj/projectexternallyedited/
---
## Prj.ProjectExternallyEdited field

Projenin dışarıdan düzenlenip düzenlenmediğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> ProjectExternallyEdited;
```

## Örnekler

Prj.ProjectExternallyEdited özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.ProjectExternallyEdited, true);

Console.WriteLine("Project Externally Edited: " + project.Get(Prj.ProjectExternallyEdited));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


