---
title: "Enum PageSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.PageSize enum. Καθορίζει το μέγεθος σελίδας"
type: docs
weight: 3250
url: /el/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Καθορίζει το μέγεθος σελίδας.

```csharp
public enum PageSize
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Letter | `0` | Το μέγεθος της σελίδας Letter σε σημεία είναι 792 × 612 |
| Ledger | `1` | Το μέγεθος της σελίδας Ledger σε σημεία είναι 1224 × 792 |
| A0 | `2` | Το μέγεθος της σελίδας A0 σε σημεία είναι 3371 × 2384 |
| A1 | `3` | Το μέγεθος της σελίδας A1 σε σημεία είναι 2384 × 1685 |
| A2 | `4` | Το μέγεθος της σελίδας A2 σε σημεία είναι 1684 × 1190 |
| A3 | `5` | Το μέγεθος της σελίδας A3 σε σημεία είναι 1190 × 842 |
| A4 | `6` | Το μέγεθος της σελίδας A4 σε σημεία είναι 842 × 595 |
| DefinedInView | `7` | Χρησιμοποιήστε το μέγεθος σελίδας που ορίζεται στο [`PageSettings`](../pagesettings/) του View (View.PageInfo.PageSettings). |

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει ότι οι υποεργασίες στη γραμμή σύνοψης εργασίας πρέπει να συγκεντρωθούν.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // Ή
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


