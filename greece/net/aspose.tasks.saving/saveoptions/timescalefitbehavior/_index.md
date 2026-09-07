---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια συμπεριφορά που καθορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το άκρο της σελίδας."
type: docs
weight: 210
url: /el/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Λαμβάνει ή ορίζει μια συμπεριφορά που καθορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το τέλος της σελίδας.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το TimescaleFitBehavior για να κάνετε την κλίμακα χρόνου του διαγράμματος Gantt να ταιριάζει στο τέλος της τελευταίας σελίδας.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Δείτε επίσης

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


