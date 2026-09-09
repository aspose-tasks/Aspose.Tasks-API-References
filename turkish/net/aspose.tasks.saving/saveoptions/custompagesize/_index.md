---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Özel sayfa boyutunu puan cinsinden alır veya ayarlar (1 point = 1/72 inç)."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Özel sayfa boyutunu nokta cinsinden alır veya ayarlar (1 nokta = inçin 1/72'si).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Örnekler

Proje PDF olarak kaydedildiğinde özel sayfa boyutunun nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


