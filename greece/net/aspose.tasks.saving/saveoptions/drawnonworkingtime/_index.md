---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί. Η προεπιλεγμένη τιμή είναι TRUE."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (Η προεπιλεγμένη τιμή είναι TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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


