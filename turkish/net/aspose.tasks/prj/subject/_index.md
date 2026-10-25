---
title: "Prj.Subject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin konusu"
type: docs
weight: 700
url: /tr/net/aspose.tasks/prj/subject/
---
## Prj.Subject field

Projenin konusu.

```csharp
public static readonly Key<string, PrjKey> Subject;
```

## Örnekler

Prj.Subject özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.Subject, "Subject");

Console.WriteLine("Subject: " + project.Get(Prj.Subject));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


