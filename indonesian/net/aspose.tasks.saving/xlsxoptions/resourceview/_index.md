---
title: "XlsxOptions.ResourceView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti XlsxOptions. Mendapatkan atau mengatur daftar kolom tampilan sumber daya untuk merender ResourceViewColumn"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/xlsxoptions/resourceview/
---
## XlsxOptions.ResourceView property

Mendapatkan atau mengatur daftar kolom tampilan sumber daya yang akan dirender ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
```

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


