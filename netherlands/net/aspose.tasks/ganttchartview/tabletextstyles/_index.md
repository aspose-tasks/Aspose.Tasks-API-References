---
title: "GanttChartView.TableTextStyles"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttChartView-eigenschap. Haalt een lijst met tabeltekststijlen op van de Gantt-diagramweergave. TableTextStyle"
type: docs
weight: 160
url: /nl/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Haalt een lijst met tabeltekststijlen op van de Gantt-diagramweergave. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## Voorbeelden

Toont hoe aangepaste tabeltekststijlen toegevoegd kunnen worden.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var view = (GanttChartView)project.Views.ToList()[0];

view.TableTextStyles.Clear();
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Red, Field = Field.TaskName });
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Gray, Field = Field.TaskDurationText });
view.TableTextStyles.Add(new TableTextStyle(2, FontStyles.Bold | FontStyles.Italic | FontStyles.Underline)
{
    Color = Color.Blue
});
```

### Zie ook

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


