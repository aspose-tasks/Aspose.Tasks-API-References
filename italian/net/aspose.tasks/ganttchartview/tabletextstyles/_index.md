---
title: "GanttChartView.TableTextStyles"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttChartView. Ottiene un elenco di stili di testo della tabella della vista Gantt Chart. TableTextStyle"
type: docs
weight: 160
url: /it/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Ottiene un elenco di stili di testo della tabella della vista Gantt Chart. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## Esempi

Mostra come aggiungere stili di testo della tabella personalizzati.

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

### Vedi anche

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


