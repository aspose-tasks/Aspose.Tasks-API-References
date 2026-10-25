---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Hesaplama ve raporlama için kullanılan tarih"
type: docs
weight: 320
url: /tr/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Hesaplama ve raporlama için kullanılan tarih.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Örnekler

Prj.ExtendedCreationDate özelliğini nasıl okuma/yazma yapacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


