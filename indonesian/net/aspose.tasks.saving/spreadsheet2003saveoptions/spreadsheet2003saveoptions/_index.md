---
title: "Spreadsheet2003SaveOptions.Spreadsheet2003SaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor Spreadsheet2003SaveOptions. Menginisialisasi sebuah instance baru dari kelas Spreadsheet2003SaveOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/spreadsheet2003saveoptions/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions constructor

Menginisialisasi sebuah instance baru dari kelas [`Spreadsheet2003SaveOptions`](../).

```csharp
public Spreadsheet2003SaveOptions()
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

* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


