---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Render edilecek sayfanın boyutunu alır veya ayarlar. Varsayılan değer PageSize.A4'tir."
type: docs
weight: 130
url: /tr/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Render edilecek sayfanın boyutunu alır veya ayarlar (Varsayılan değer PageSize.A4'tür).

```csharp
public PageSize PageSize { get; set; }
```

## Örnekler

Sayfa boyutunun nasıl ayarlanacağını gösterir ( &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt; enumarasyonunun değerlerinden biri olabilir).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Projeyi tüm Önceden Tanımlı sayfa boyutlarına render edin.
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### Ayrıca Bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


