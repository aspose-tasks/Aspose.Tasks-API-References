---
title: "Enum PresentationFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. Enumeratie voor presentatieformaat"
type: docs
weight: 3270
url: /nl/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Enumeratie voor presentatieformaat.

```csharp
public enum PresentationFormat
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| GanttChart | `0` | Presentatieformaat voor Gantt-diagram. |
| TaskUsage | `1` | Presentatieformaat voor taakgebruik. |
| ResourceUsage | `2` | Presentatieformaat voor resourcegebruik. |
| ResourceSheet | `3` | Presentatieformaat voor resourcesheet. |
| TaskSheet | `4` | Presentatieformaat voor taakblad. |

## Voorbeelden

Toont hoe de weergave van het resourcesheet wordt gerenderd.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Stel het presentatieformaat in op Resourcesheet
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


