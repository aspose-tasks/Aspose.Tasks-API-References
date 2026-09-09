---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. İlerlemeyi göstermek veya kazanılmış değer toplamlarını hesaplamak için durum tarihi. Durum tarihi, farklı bir tarih belirtilmedikçe mevcut tarih (bugünün tarihi) ile aynıdır."
type: docs
weight: 690
url: /tr/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

İlerlemeyi görüntülemek veya kazanılmış değer toplamlarını hesaplamak için durum tarihi. Durum tarihi, farklı bir durum tarihi belirtilmedikçe geçerli tarih (bugünün tarihi) ile aynıdır.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Örnekler

Prj.StatusDate özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


