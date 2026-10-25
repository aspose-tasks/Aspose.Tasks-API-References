---
title: "UseProjectDefaultFont"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta un valore che indica se il carattere predefinito deve essere usato per il rendering."
type: docs
weight: 120
url: /it/net/aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/
---
## PdfSaveOptions.UseProjectDefaultFont property

Ottiene o imposta un valore che indica se il carattere predefinito deve essere usato per il rendering.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Osservazioni

Quando il valore è False e DefaultFontName è specificato, il motore di rendering utilizzerà il carattere specificato da DefaultFontName come carattere di riserva. Altrimenti vengono utilizzati come carattere di riserva 'Arial' (se installato) o i caratteri 'Generic Sans Serif'. Il carattere di riserva viene utilizzato durante il rendering della vista del progetto quando uno stile di testo fa riferimento a un carattere non installato sul sistema operativo corrente. Per un maggiore controllo sulla risoluzione dei caratteri è possibile utilizzare il callback [`FontResolveCallback`](../fontresolvecallback).

### Esempi

Mostra come impostare un font personalizzato che verrà usato per la stampa del PDF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Vedi anche

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
