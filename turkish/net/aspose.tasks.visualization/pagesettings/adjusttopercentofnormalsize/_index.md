---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageSettings özelliği. Yazdırmayı belirtilen yüzde (PercentOfNormalSize) normal boyuta ayarlayıp ayarlamama durumunu gösteren bir değeri alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Yazdırmayı belirtilen yüzde ([`PercentOfNormalSize`](../percentofnormalsize/)) normal boyuta ayarlayıp ayarlamama durumunu gösteren bir değeri alır veya ayarlar.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Açıklamalar

Proje HTML formatında render edildiğinde etkili değildir.

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


