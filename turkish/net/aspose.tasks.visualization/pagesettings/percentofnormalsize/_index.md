---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageSettings özelliği. Yazdırmayı ayarlamak için normal boyutun bir yüzdesini alır veya ayarlar."
type: docs
weight: 90
url: /tr/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Yazdırmayı ayarlamak için normal boyutun yüzdesini alır veya ayarlar.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Örnekler

Belirtilen ölçek faktörüyle görünümün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// Görünümün belirtilen ölçek faktörü kullanılarak ölçeklendirilmesi gerektiğini gösteren bir değer ayarlayın.
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// ölçek faktörünü belirtin.
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


