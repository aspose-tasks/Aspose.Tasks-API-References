---
title: "PageSettings.PaperSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageSettings özelliği. Bir kağıt boyutu alır veya ayarlar. PrinterPaperSize enumarasyonunun değerlerinden biri olabilir."
type: docs
weight: 70
url: /tr/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

Bir kağıt boyutu alır veya ayarlar. [`PrinterPaperSize`](../../printerpapersize/) enumarasyonunun değerlerinden biri olabilir.

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

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

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


