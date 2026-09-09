---
title: "PageViewSettings.PrintBlankPages"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageViewSettings özelliği. Görünümün boş sayfalarını yazdırıp yazdırmayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks.visualization/pageviewsettings/printblankpages/
---
## PageViewSettings.PrintBlankPages property

Bir görünümün boş sayfalarının yazdırılıp yazdırılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool PrintBlankPages { get; set; }
```

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

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


