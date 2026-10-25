---
title: "Enum PageSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageSize enum. Specificeert paginagrootte"
type: docs
weight: 3250
url: /nl/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Specificeert paginagrootte.

```csharp
public enum PageSize
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Letter | `0` | De grootte van de Letter-pagina in punten is 792 × 612 |
| Ledger | `1` | De grootte van de Ledger-pagina in punten is 1224 × 792 |
| A0 | `2` | De grootte van de A0-pagina in punten is 3371 × 2384 |
| A1 | `3` | De grootte van de A1-pagina in punten is 2384 × 1685 |
| A2 | `4` | De grootte van de A2-pagina in punten is 1684 × 1190 |
| A3 | `5` | De grootte van de A3-pagina in punten is 1190 × 842 |
| A4 | `6` | De grootte van de A4-pagina in punten is 842 × 595 |
| DefinedInView | `7` | Gebruik paginagrootte gedefinieerd in View's [`PageSettings`](../pagesettings/) (View.PageInfo.PageSettings). |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


