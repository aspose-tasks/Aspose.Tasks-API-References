---
title: "GanttChartView.TextStyles"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttChartView. Mendapatkan atau mengatur daftar TextStyle dari tampilan Gantt Chart"
type: docs
weight: 170
url: /id/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Mendapatkan atau mengatur daftar [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) dari tampilan Gantt Chart.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Contoh

Menampilkan cara membaca gaya teks Gantt chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// iterasi atas gaya teks dari tampilan Gantt chart
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Lihat Juga

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


