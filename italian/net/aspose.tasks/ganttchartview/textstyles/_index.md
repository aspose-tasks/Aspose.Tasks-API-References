---
title: "GanttChartView.TextStyles"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttChartView. Ottiene o imposta un elenco di TextStyle della vista Gantt Chart"
type: docs
weight: 170
url: /it/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Ottiene o imposta un elenco di [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) della vista Gantt Chart.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Esempi

Mostra come leggere gli stili di testo del diagramma di Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// itera sugli stili di testo della vista del diagramma di Gantt
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Vedi anche

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


