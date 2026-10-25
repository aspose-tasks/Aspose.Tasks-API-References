---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Satır yüksekliğinin içeriğine sığacak şekilde artırılıp artırılmayacağını belirten bir değeri alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool FitContent { get; set; }
```

## Örnekler

Satır yüksekliğinin içeriğine uyacak şekilde artırılıp artırılmayacağını ayarlama seçeneğinin nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // İçeriği sığdırma seçeneğini true olarak ayarla
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


