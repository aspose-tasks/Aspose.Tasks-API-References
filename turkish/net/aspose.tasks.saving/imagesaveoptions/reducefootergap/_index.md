---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. Son görev ile altbilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri alır veya ayarlar."
type: docs
weight: 80
url: /tr/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Örnekler

Son görev ile altbilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Görevler listesi ile Altbilgi arasındaki boşluğu azaltmak için ReduceFooterGap özelliğini kullanın.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


