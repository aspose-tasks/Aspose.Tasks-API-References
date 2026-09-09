---
title: "Prj.Category"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin kategorisi"
type: docs
weight: 100
url: /tr/net/aspose.tasks/prj/category/
---
## Prj.Category field

Bir projenin kategorisi.

```csharp
public static readonly Key<string, PrjKey> Category;
```

## Örnekler

Prj.Category özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.Category, "Special");

Console.WriteLine("Category: " + project.Get(Prj.Category));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


