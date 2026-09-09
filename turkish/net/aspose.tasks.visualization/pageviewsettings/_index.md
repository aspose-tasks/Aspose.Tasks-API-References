---
title: "Sınıf PageViewSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageViewSettings sınıfı. Bir proje görünümü için yazdırma ayarlarını temsil eder."
type: docs
weight: 3260
url: /tr/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Proje görünümü için yazdırma ayarlarını temsil eder.

```csharp
public class PageViewSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Tüm sayfalarda yazdırılacak ilk sütun sayısını alır veya ayarlar. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Yazdırma sırasında zaman ölçeğinin bir sayfanın sonuna sığdırılıp sığdırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Bir görünümün tüm sayfa sütunlarının yazdırılıp yazdırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Bir görünümün boş sayfalarının yazdırılıp yazdırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Tüm sayfalarda belirtilen sayıda ilk sütunun yazdırılıp yazdırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Notların yazdırılıp yazdırılmayacağını gösteren bir değeri alır veya ayarlar. |

## Örnekler

Görev, kaynak ve atama notlarını ayrı bir sayfada nasıl yazdıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "Input.mpp");

// tüm sayfalarda yazdırılacak ilk sütun sayısını ayarla
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// Notların yazdırılıp yazdırılmayacağını gösteren bir değeri ayarlar.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// Yazdırma sırasında zaman ölçeğinin bir sayfanın sonuna sığdırılıp sığdırılmayacağını gösteren bir değeri ayarlar.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// Bir görünümün tüm sayfa sütunlarının yazdırılıp yazdırılmayacağını gösteren bir değeri ayarlar
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// Bir görünümün boş sayfalarının yazdırılıp yazdırılmayacağını gösteren bir değeri ayarlar
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// tüm sayfalarda belirli sayıda ilk sütunun yazdırılıp yazdırılmayacağını belirten bir değer ayarla
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


