---
title: "Enum PageSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. Specifica la dimensione della pagina"
type: docs
weight: 3250
url: /it/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Specifica la dimensione della pagina.

```csharp
public enum PageSize
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Letter | `0` | La dimensione della pagina Letter in punti è 792 × 612 |
| Ledger | `1` | La dimensione della pagina Ledger in punti è 1224 × 792 |
| A0 | `2` | La dimensione della pagina A0 in punti è 3371 × 2384 |
| A1 | `3` | La dimensione della pagina A1 in punti è 2384 × 1685 |
| A2 | `4` | La dimensione della pagina A2 in punti è 1684 × 1190 |
| A3 | `5` | La dimensione della pagina A3 in punti è 1190 × 842 |
| A4 | `6` | La dimensione della pagina A4 in punti è 842 × 595 |
| DefinedInView | `7` | Utilizza la dimensione della pagina definita in [`PageSettings`](../pagesettings/) della View (View.PageInfo.PageSettings). |

## Esempi

Mostra come impostare un valore che indica che le sottoattività sulla barra dell'attività di riepilogo devono essere aggregate.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OPPURE
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


