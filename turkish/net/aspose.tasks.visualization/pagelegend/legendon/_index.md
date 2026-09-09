---
title: "PageLegend.LegendOn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageLegend özelliği. Açıklamanın göründüğü sayfaları alır veya ayarlar. Legend sayımının değerlerinden biri olabilir."
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

Açıklamanın göründüğü sayfaları alır veya ayarlar. [`Legend`](../../legend/) sayımının değerlerinden biri olabilir.

```csharp
public Legend LegendOn { get; set; }
```

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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


