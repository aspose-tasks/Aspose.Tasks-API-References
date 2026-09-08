---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt de paginagrootte op of stelt deze in die gerenderd moet worden. Standaardwaarde is PageSize.A4"
type: docs
weight: 130
url: /nl/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Haalt op of stelt de grootte van de te renderen pagina in (Standaardwaarde is PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Voorbeelden

Toont hoe de paginagrootte in te stellen (kan een van de waarden van de &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt; enumeratie zijn).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Render het project naar alle vooraf gedefinieerde paginagroottes
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

### Zie ook

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


