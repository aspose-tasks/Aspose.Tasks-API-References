---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GanttChartView. Λαμβάνει ή ορίζει μια λίστα των TextStyle της προβολής Gantt Chart"
type: docs
weight: 170
url: /el/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Λαμβάνει ή ορίζει μια λίστα των [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) της προβολής Gantt Chart.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα στυλ κειμένου του Gantt chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// επανάληψη πάνω στα στυλ κειμένου της προβολής Gantt chart
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Δείτε επίσης

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


