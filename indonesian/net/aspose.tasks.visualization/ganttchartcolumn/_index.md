---
title: "Kelas GanttChartColumn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.GanttChartColumn. Kelas tampilan proyek"
type: docs
weight: 3090
url: /id/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Kelas tampilan proyek

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Menginisialisasi instansi baru dari kelas GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Menginisialisasi instansi baru dari kelas GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Menginisialisasi instansi baru dari kelas GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Menginisialisasi instansi baru dari kelas GanttChartColumn. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Kolom bidang. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Mendapatkan nama kolom. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Mendapatkan atau mengatur perataan teks (bisa menjadi salah satu nilai dari enumerasi [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Mendapatkan lebar kolom. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Mengonversi tugas saat ini menjadi teks kolom. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


