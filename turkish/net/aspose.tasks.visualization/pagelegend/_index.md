---
title: "Sınıf PageLegend"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageLegend sınıfı. Proje yazdırma için kullanılan bir sayfa lejandını temsil eder."
type: docs
weight: 3210
url: /tr/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Proje yazdırma için kullanılan bir sayfa lejandını temsil eder.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageLegend](pagelegend/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Üst öğede görüntülenecek ortalanmış resmi alır veya ayarlar. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Ortadaki görüntünün gösterilen boyutunu alır veya ayarlar. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Üst öğede görüntülenecek ortalanmış metni alır veya ayarlar. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Üst öğede görüntülenecek sola hizalanmış resmi alır veya ayarlar. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Sol resmin görüntülenen boyutunu alır veya ayarlar. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Üst öğede görüntülenecek sola hizalanmış metni alır veya ayarlar. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Lejandın göründüğü sayfaları alır veya ayarlar. [`Legend`](../legend/) enumarasyonunun değerlerinden biri olabilir. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Üst öğede görüntülenecek sağa hizalanmış resmi alır veya ayarlar. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Sağ resmin görüntülenen boyutunu alır veya ayarlar. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Üst öğede görüntülenecek sağa hizalanmış metni alır veya ayarlar. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Lejandın sol kısmının (varsayılan olarak projenin adı ve tarihini içerir) genişliğini santimetre cinsinden alır veya ayarlar. |

## Örnekler

Sayfa lejand bilgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// sayfa lejand bilgilerini okuyalım
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// aynı zamanda bir lejandın değiştirilmesi de desteklenir
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


