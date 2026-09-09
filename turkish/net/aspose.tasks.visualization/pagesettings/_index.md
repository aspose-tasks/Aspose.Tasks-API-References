---
title: "Sınıf PageSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageSettings sınıfı. Proje görünümünün bir sayfası için baskı ayarlarını temsil eder"
type: docs
weight: 3240
url: /tr/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Proje görünümünün bir sayfası için yazdırma ayarlarını temsil eder.

```csharp
public class PageSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageSettings](pagesettings/)() | `PageSettings` sınıfının yeni bir örneğini başlatır. Proje görünümünün bir sayfası için baskı ayarlarını temsil eder. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Yazdırmayı normal boyutun belirtilen yüzdesine ([`PercentOfNormalSize`](./percentofnormalsize/)) ayarlayıp ayarlamayacağını gösteren bir değeri alır veya ayarlar. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Yazdırma için ilk sayfa numarasını alır veya ayarlar. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Sayfa yönünün dikey olup olmadığını gösteren bir değeri alır veya ayarlar; sayfa yönü yataysa false döndürür. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Yazdırılacak yükseklik sayfa sayısını alır veya ayarlar. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Yazdırılacak genişlik sayfa sayısını alır veya ayarlar. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Kağıt boyutunu alır veya ayarlar. [`PrinterPaperSize`](../printerpapersize/) enum değerlerinden biri olabilir. |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tam sayı alır veya ayarlar. Bu değer, OS ayarlarından PaperSize'ı almak için kullanılabilir. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Yazdırmayı ayarlamak için normal boyutun yüzdesini alır veya ayarlar. |

## Örnekler

&lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt; ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// ayarları al
var settings = project.DefaultView.PageInfo.PageSettings;
// bazı özellikleri ayarlayalım
// Sayfa yönünün portre olup olmadığını gösteren bir değeri ayarlar; sayfa yönü yataysa false döndürür.
settings.IsPortrait = true;
// Yazdırılacak genişlik sayfa sayısını ayarlar.
settings.PagesInWidth = 5;
// Yazdırılacak yükseklik sayfa sayısını ayarlar.
settings.PagesInHeight = 7;
// Yazdırmayı ayarlamak için normal boyutun yüzdesini ayarlar.
settings.PercentOfNormalSize = 200;
// kağıt boyutunu ayarlar. <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" /> enum değerlerinden biri olabilir.
settings.PaperSize = PrinterPaperSize.PaperB4;
// Yazdırma için ilk sayfa numarasını ayarlar.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


