---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView-eigenschap. Haalt een lijst met TextStyle op of stelt deze in voor de Gantt-diagramweergave"
type: docs
weight: 170
url: /nl/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Haalt een lijst met [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) op of stelt deze in voor de Gantt-diagramweergave.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Voorbeelden

Toont hoe Gantt-diagramtekststijlen gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// itereren over tekststijlen van de Gantt-diagramweergave
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Zie ook

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


