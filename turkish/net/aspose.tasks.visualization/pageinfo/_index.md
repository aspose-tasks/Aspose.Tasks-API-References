---
title: "Sınıf PageInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageInfo sınıfı. MPP dosya formatında bulunan ve yazdırma için kullanılan sayfa ayarı verilerini temsil eder."
type: docs
weight: 3200
url: /tr/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

MPP dosya formatında bulunan ve yazdırma için kullanılan sayfa ayarı verilerini temsil eder.

```csharp
public class PageInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageInfo](pageinfo/)() | `PageInfo` sınıfının yeni bir örneğini başlatır. MPP dosya formatında bulunan ve yazdırma için kullanılan sayfa ayarı verilerini temsil eder. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Alt bilgi verisini temsil eden [`HeaderFooterInfo`](../headerfooterinfo/) sınıfının bir örneğini alır veya ayarlar. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Üst bilgi verisini temsil eden [`HeaderFooterInfo`](../headerfooterinfo/) sınıfının bir örneğini alır veya ayarlar. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Sayfa lejandının renderleme seçeneklerini belirten [`PageLegend`](../pagelegend/) sınıfının bir örneğini alır veya ayarlar. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | [`PageMargins`](../pagemargins/) sınıfının sayfa kenar boşluklarını belirten bir örneğini alır. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Kurulum verilerinin kullanıldığı görünümün adını alır. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | [`PageSettings`](./pagesettings/) sınıfının sayfa yazdırma ayarlarını belirten bir örneğini alır. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | [`PageViewSettings`](./pageviewsettings/) sınıfının sayfa görünümü yazdırma ayarlarını belirten bir örneğini alır. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


