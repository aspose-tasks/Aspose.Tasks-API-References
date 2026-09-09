---
title: "Sınıf PageMargins"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageMargins sınıfı. Baskı için sayfa kenar boşluklarını temsil eder"
type: docs
weight: 3230
url: /tr/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Yazdırma için sayfa kenar boşluklarını temsil eder.

```csharp
public class PageMargins
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageMargins](pagemargins/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Kenarlıkları yazdırılacak konumu alır veya ayarlar. [`Border`](../border/) enumarasyonunun değerlerinden biri olabilir. |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Alt kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Sol kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Sağ kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Üst kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar. |

## Örnekler

Sayfa kenar boşluklarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// varsayılan görünümü değiştirelim
var margins = project.DefaultView.PageInfo.Margins;

// kenar boşluklarını değiştirelim
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


