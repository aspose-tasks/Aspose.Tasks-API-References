---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Geeft een waarde op die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen."
type: docs
weight: 50
url: /nl/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Haalt op of stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen.

```csharp
public bool FitContent { get; set; }
```

## Voorbeelden

Toont hoe de optie in te stellen of de rijhoogte moet worden vergroot om de inhoud te passen.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Stel optie fit content in op true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


