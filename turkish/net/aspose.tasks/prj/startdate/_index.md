---
title: "Prj.StartDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin başlangıç tarihi"
type: docs
weight: 680
url: /tr/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

Bir projenin başlangıç tarihi.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Örnekler

Prj.StartDate özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


