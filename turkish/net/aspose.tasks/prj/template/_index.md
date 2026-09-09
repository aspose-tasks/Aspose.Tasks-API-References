---
title: "Prj.Template"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Proje şablonu"
type: docs
weight: 720
url: /tr/net/aspose.tasks/prj/template/
---
## Prj.Template field

Projenin şablonu.

```csharp
public static readonly Key<string, PrjKey> Template;
```

## Örnekler

Prj.Template özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.Template, "Custom Template");

Console.WriteLine("Template: " + project.Get(Prj.Template));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


