---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectView. Περιλαμβάνει στήλες εργασιών id, ενδείξεις, όνομα, διάρκεια, έναρξη, λήξη, προγενέστερα και ονόματα πόρων"
type: docs
weight: 60
url: /el/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Περιλαμβάνει στήλες εργασίας id, indicators, name, duration, start, finish, predecessors και resource names.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Τιμή Επιστροφής

Μια προβολή που περιέχει μια λίστα του [`GanttChartColumn`](../../ganttchartcolumn/).

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή φύλλου εργασιών.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Δείτε επίσης

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


