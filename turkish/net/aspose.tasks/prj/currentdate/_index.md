---
title: "Prj.CurrentDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Sistem tarihi"
type: docs
weight: 190
url: /tr/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

Sistem tarihi.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Örnekler

Prj.CurrentDate özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


