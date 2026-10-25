---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "HtmlSaveOptions özelliği. Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını belirten bir değeri alır veya ayarlar."
type: docs
weight: 150
url: /tr/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Örnekler

HTML çıktı dosyalarında son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını belirten bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


