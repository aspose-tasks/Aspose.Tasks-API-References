---
title: "Kelas Spreadsheet2003SaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.Spreadsheet2003SaveOptions. Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke Spreadsheet2003"
type: docs
weight: 2220
url: /id/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Mengizinkan untuk menentukan opsi tambahan saat merender halaman proyek ke Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | Menginisialisasi instance baru dari kelas `Spreadsheet2003SaveOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan penugasan yang akan dirender ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan sumber daya yang akan dirender ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) yang akan disimpan. Jika tidak diatur, maka kolom default akan disimpan. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


