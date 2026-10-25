---
title: "SaveOptions.PageSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta la dimensione della pagina da renderizzare. Il valore predefinito è PageSize.A4"
type: docs
weight: 130
url: /it/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Ottiene o imposta la dimensione della pagina da renderizzare (Il valore predefinito è PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Esempi

Mostra come impostare la dimensione della pagina (può essere uno dei valori dell'enumerazione &lt;see cref=\"P:Aspose.Tasks.Visualization.TiffCompression\" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Renderizza il progetto in tutte le dimensioni di pagina predefinite
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

### Vedi anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


