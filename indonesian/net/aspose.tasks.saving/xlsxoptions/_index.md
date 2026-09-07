---
title: "Kelas XlsxOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.XlsxOptions. Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke XLSX."
type: docs
weight: 2270
url: /id/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Menginisialisasi instance baru dari kelas `XlsxOptions` yang dapat digunakan untuk menyimpan proyek dalam format XLSX. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan penugasan yang akan dirender ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Mendapatkan atau mengatur enkoding file XLSX yang dihasilkan. Nilai default adalah UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan sumber daya yang akan dirender ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) untuk disimpan dalam format XLSX. Jika tidak diatur, maka kolom default akan disimpan. |

## Contoh

Menampilkan cara menyimpan proyek ke file XLSX dengan menggunakan opsi &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Tambahkan kolom Gantt Chart yang diinginkan
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Tambahkan kolom tampilan sumber daya yang diinginkan
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Tambahkan kolom tampilan penugasan yang diinginkan
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// atur enkoding
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


