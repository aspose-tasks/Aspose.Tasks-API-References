---
title: "GanttChartColumn.GetColumnText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "GanttChartColumn metode. Mengonversi tugas saat ini menjadi teks kolom"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/ganttchartcolumn/getcolumntext/
---
## GanttChartColumn.GetColumnText method

Mengonversi tugas saat ini menjadi teks kolom.

```csharp
public string GetColumnText(Task task)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | Tugas | Tugas saat ini. |

### Nilai Kembali

Teks kolom.

## Contoh

Menampilkan cara menambahkan kolom tampilan diagram Gantt untuk diekspor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// iterasi melalui kolom
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


