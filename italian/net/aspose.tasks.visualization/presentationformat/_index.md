---
title: "Enum PresentationFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "**Aspose.Tasks.Visualization.PresentationFormat** enum. Enumerazione per il formato di presentazione"
type: docs
weight: 3270
url: /it/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Enumerazione per il formato di presentazione.

```csharp
public enum PresentationFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| GanttChart | `0` | Formato di presentazione del diagramma di Gantt. |
| TaskUsage | `1` | Formato di presentazione dell'utilizzo delle attività. |
| ResourceUsage | `2` | Formato di presentazione dell'utilizzo delle risorse. |
| ResourceSheet | `3` | Formato di presentazione del foglio risorse. |
| TaskSheet | `4` | Formato di presentazione del foglio attività. |

## Esempi

Mostra come rendere la vista del foglio risorse.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Imposta il Formato di Presentazione su Foglio risorse
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


