---
title: "Spreadsheet2003SaveOptions.AssignmentView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Spreadsheet2003SaveOptions. Mendapatkan atau mengatur daftar kolom tampilan penugasan untuk merender AssignmentViewColumn"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/
---
## Spreadsheet2003SaveOptions.AssignmentView property

Mendapatkan atau mengatur daftar kolom tampilan penugasan untuk merender ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

## Contoh

Menampilkan cara menambahkan kolom yang akan diekspor selama mengekspor proyek ke format Spreadsheet2003.

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

### Lihat Juga

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


