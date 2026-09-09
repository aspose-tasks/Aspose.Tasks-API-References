---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageSettings özelliği. Sayfa yönünün portre olup olmadığını gösteren bir değeri alır veya ayarlar; sayfa yönü yatay ise false döndürür."
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Sayfa yönünün dikey olup olmadığını gösteren bir değeri alır veya ayarlar; sayfa yönü yataysa false döndürür.

```csharp
public bool IsPortrait { get; set; }
```

## Açıklamalar

SaveOptions.PageSize == Visualization.PageSize.DefinedInView olduğunda render sırasında uygulanır.

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

View ayarlarını veya SaveOptions'ı kullanarak sayfa boyutu ve yönünün nasıl belirtileceğini gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Bu durumda sayfa boyutu ve yönü, view.PageInfo.PageSettings.PaperSize ve view.PageInfo.PageSettings.IsPortrait özelliklerinden uygulanır.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Bu durumda sayfa boyutu ve yönü, SaveOptions özelliklerinden uygulanır.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Bu durumda sayfa boyutu, SaveOptions.CustomPageSize'tan uygulanır. IsPortrait özelliği dikkate alınmaz.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Ayrıca Bakınız

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


