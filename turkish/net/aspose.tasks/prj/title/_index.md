---
title: "Prj.Title"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin başlığı"
type: docs
weight: 750
url: /tr/net/aspose.tasks/prj/title/
---
## Prj.Title field

Bir projenin başlığı.

```csharp
public static readonly Key<string, PrjKey> Title;
```

## Örnekler

Prj.Title özelliğini nasıl okuma/yazma yapacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.Title, "MS Project");

Console.WriteLine("Title: " + project.Get(Prj.Title));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


