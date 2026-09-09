---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin oluşturulduğu tarih ve saat"
type: docs
weight: 130
url: /tr/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

Projenin oluşturulduğu tarih ve saat.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Açıklamalar

mpp dosyalarında UTC formatında kaydedilir. DateTime türü.

## Örnekler

Prj.CreationDate özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


