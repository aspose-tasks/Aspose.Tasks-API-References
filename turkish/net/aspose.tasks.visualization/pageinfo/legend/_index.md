---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageInfo özelliği. Sayfa lejandının renderleme seçeneklerini belirten PageLegend sınıfının bir örneğini alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Sayfa lejandının renderleme seçeneklerini belirten [`PageLegend`](../../pagelegend/) sınıfının bir örneğini alır veya ayarlar.

```csharp
public PageLegend Legend { get; set; }
```

## Açıklamalar

Şu anda yalnızca Gantt Şeması görünümlerine uygulanabilir.

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

MS Project görünümünün sayfa bilgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// varsayılan görünümü değiştirelim
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// kenar boşluklarını değiştirelim
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// sayfa ayarlarını değiştirelim
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// sayfa görünüm ayarlarını değiştirelim
// Notların yazdırılıp yazdırılmayacağını gösteren bir değeri ayarlar.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// projeyle çalış...
```

### Ayrıca Bakınız

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


