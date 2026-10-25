---
title: "PageInfo.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageInfo özelliği. Ayar verilerinin kullanıldığı görünümün adını alır"
type: docs
weight: 60
url: /tr/net/aspose.tasks.visualization/pageinfo/name/
---
## PageInfo.Name property

Kurulum verilerinin kullanıldığı görünümün adını alır.

```csharp
public string Name { get; }
```

## Örnekler

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


