---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Sayfa yönünün portre olup olmadığını belirten bir değeri alır veya ayarlar; sayfa yönü yatay ise false döndürür."
type: docs
weight: 70
url: /tr/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Sayfa yönünün dikey olup olmadığını gösteren bir değeri alır veya ayarlar; sayfa yönü yataysa false döndürür.

```csharp
public bool IsPortrait { get; set; }
```

## Açıklamalar

SaveOptions.PageSize == Visualization.PageSize.DefinedInView olduğunda uygulanmaz. Bu durumda View.PageInfo.PageSettings.IsPortrait kullanılır. SaveOptions.CustomPageSize ayarlandığında da uygulanmaz.

## Örnekler

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


