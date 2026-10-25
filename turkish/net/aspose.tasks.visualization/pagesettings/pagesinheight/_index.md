---
title: "PageSettings.PagesInHeight"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageSettings özelliği. Yazdırılacak yükseklikteki sayfa sayısını alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Yazdırılacak yükseklik sayfa sayısını alır veya ayarlar.

```csharp
public int PagesInHeight { get; set; }
```

## Örnekler

'Fit X to Y pages' seçeneğiyle görünümün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// Görünümün yükseklikte 2 sayfadan az veya eşit olarak oluşturulması gerektiğini belirtin.
view.PageInfo.PageSettings.PagesInHeight = 2;
// Görünümün genişlikte 1 sayfada oluşturulması gerektiğini belirtin.
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


