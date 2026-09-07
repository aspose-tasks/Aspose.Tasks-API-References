---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα υπο-εργα σε γραμμή σύνοψης εργασίας πρέπει να σημειωθούν. Για τα υπο-εργα το πεδίο Rollup υποδεικνύει εάν οι πληροφορίες για τις γραμμές Gantt των υπο-εργα θα ενσωματωθούν στη γραμμή σύνοψης εργασίας. Για τις εργασίες σύνοψης το πεδίο Rollup υποδεικνύει εάν η γραμμή σύνοψης εργασίας εμφανίζει ενσωματωμένες γραμμές. Πρέπει να έχετε το πεδίο Rollup για τις εργασίες σύνοψης ορισμένο σε Ναι ώστε οποιαδήποτε υπο-εργα να ενσωματωθούν σε αυτές."
type: docs
weight: 160
url: /el/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν οι υποεργασίες στη μπάρα της συνολικής εργασίας πρέπει να σημειωθούν. Για τις υποεργασίες, το πεδίο Rollup υποδεικνύει εάν οι πληροφορίες στις μπαρ Gantt των υποεργασιών θα ενσωματωθούν στη μπάρα της συνολικής εργασίας. Για τις συνολικές εργασίες, το πεδίο Rollup υποδεικνύει εάν η μπάρα της συνολικής εργασίας εμφανίζει ενσωματωμένες μπαρ. Πρέπει να έχετε το πεδίο Rollup για τις συνολικές εργασίες ορισμένο σε Yes ώστε οποιεσδήποτε υποεργασίες να ενσωματωθούν σε αυτές.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Παρατηρήσεις

Ισχύει μόνο όταν η προβολή Gantt chart αποδίδεται.

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


