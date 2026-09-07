---
title: "Spreadsheet2003SaveOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Spreadsheet2003SaveOptions. Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση AssignmentViewColumn."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/
---
## Spreadsheet2003SaveOptions.AssignmentView property

Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες που θα εξαχθούν κατά την εξαγωγή του έργου σε μορφή Spreadsheet2003.

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
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


