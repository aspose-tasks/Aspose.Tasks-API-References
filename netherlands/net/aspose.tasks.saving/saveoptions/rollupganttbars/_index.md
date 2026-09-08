---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de subtaak‑Gantt‑balken wordt opgehoogd naar de samenvattingsbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingsbalk opgehoogde balken weergeeft. U moet het Rollup‑veld voor samenvattingstaken op Ja instellen zodat subtaken naar hen kunnen worden opgehoogd."
type: docs
weight: 160
url: /nl/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Haalt op of stelt een waarde in die aangeeft of subtaken op de samenvattingstaakbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgerold naar de samenvattingstaakbalk. Voor samenvattingstaken geeft het Rollup‑veld aan of de samenvattingstaakbalk opgerolde balken weergeeft. Het Rollup‑veld voor samenvattingstaken moet op Ja staan om subtaken naar hen op te rollen.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Opmerkingen

Is alleen van toepassing wanneer de Gantt‑chartweergave wordt gerenderd.

## Voorbeelden

Toont hoe een waarde in te stellen die aangeeft dat subtaken op de samenvattingstaakbalk moeten worden opgeteld.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OF
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


