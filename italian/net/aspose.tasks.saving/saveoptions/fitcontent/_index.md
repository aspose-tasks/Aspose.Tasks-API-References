---
title: "SaveOptions.FitContent"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al suo contenuto"
type: docs
weight: 50
url: /it/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Ottiene o imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto.

```csharp
public bool FitContent { get; set; }
```

## Esempi

Mostra come impostare l'opzione per aumentare l'altezza della riga in modo da adattarla al contenuto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Imposta l'opzione fit content su true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


