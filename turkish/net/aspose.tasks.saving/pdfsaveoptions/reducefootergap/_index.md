---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Örnekler

PDF çıktı dosyalarında son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını belirten bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


