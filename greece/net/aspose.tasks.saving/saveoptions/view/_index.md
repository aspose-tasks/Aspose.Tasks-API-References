---
title: "SaveOptions.View"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής για απόδοση GanttChartColumn. Εάν δεν οριστεί, τότε αποδίδονται μόνο τα IDs εργασιών, τα ονόματα εργασιών, η έναρξη και το τέλος. Εάν οριστούν και οι ιδιότητες View και ViewSettings, οι στήλες από το View παρακάμπτουν τις στήλες από το ViewSettings."
type: docs
weight: 230
url: /el/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής για απόδοση ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Εάν δεν οριστεί, τότε αποδίδονται μόνο τα IDs εργασιών, τα ονόματα εργασιών, η έναρξη και το τέλος. Εάν οριστούν και οι ιδιότητες View και [`ViewSettings`](../viewsettings/), οι στήλες από το View παρακάμπτουν τις στήλες από το ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής που θα εξαχθούν κατά την εξαγωγή του έργου.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Δείτε επίσης

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


