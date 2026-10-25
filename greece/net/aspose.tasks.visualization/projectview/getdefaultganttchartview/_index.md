---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectView. Περιλαμβάνει στήλες εργασιών id, ενδείξεις, όνομα, διάρκεια, έναρξη και λήξη"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Περιλαμβάνει στήλες id, δείκτες, όνομα, διάρκεια, έναρξη και λήξη εργασίας.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Τιμή Επιστροφής

Μια προβολή που περιέχει μια λίστα του [`GanttChartColumn`](../../ganttchartcolumn/).

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή Gantt chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Δείτε επίσης

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


