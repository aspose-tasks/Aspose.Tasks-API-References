---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà FontSettings. Ottiene o imposta un valore che indica se il font predefinito deve essere usato per il rendering"
type: docs
weight: 40
url: /it/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Ottiene o imposta un valore che indica se il carattere predefinito deve essere usato per il rendering.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Osservazioni

Quando il valore è False e DefaultFontName è specificato, il motore di rendering utilizzerà il carattere specificato da DefaultFontName come carattere di riserva. Altrimenti vengono utilizzati 'Arial' (se installato) o i caratteri 'Generic Sans Serif' come carattere di riserva. Il carattere di riserva è utilizzato durante il rendering della vista progetto quando uno stile di testo fa riferimento a un carattere non installato sul sistema operativo corrente. Per un controllo maggiore sulla risoluzione dei caratteri è possibile utilizzare il callback [`FontResolveCallback`](../fontresolvecallback/).

## Esempi

Mostra come impostare un font personalizzato che verrà usato per la stampa del PDF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Vedi anche

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


