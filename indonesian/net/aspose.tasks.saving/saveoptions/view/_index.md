---
title: "SaveOptions.View"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur daftar kolom view yang akan dirender GanttChartColumn. Jika tidak diatur, hanya ID tugas, nama tugas, mulai, dan selesai yang akan dirender. Jika kedua properti View dan ViewSettings diatur, kolom dari View akan menggantikan kolom dari ViewSettings."
type: docs
weight: 230
url: /id/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Mendapatkan atau mengatur daftar kolom view yang akan dirender ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Jika tidak diatur, hanya ID tugas, nama tugas, mulai, dan selesai yang akan dirender. Jika kedua properti View dan [`ViewSettings`](../viewsettings/) diatur, kolom dari View akan menggantikan kolom dari ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Contoh

Menampilkan cara menambahkan kolom view yang akan diekspor selama proses ekspor proyek.

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


