---
title: "ProjectView.ProjectView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ProjectView. Menginisialisasi instance baru dari kelas ProjectView"
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

Menginisialisasi instance baru dari kelas [`ProjectView`](../).

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kolom | IEnumerable`1 | Daftar kolom tampilan. |

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan yang memiliki kumpulan kolom khusus.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// iterasi kolom tampilan
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Lihat Juga

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


