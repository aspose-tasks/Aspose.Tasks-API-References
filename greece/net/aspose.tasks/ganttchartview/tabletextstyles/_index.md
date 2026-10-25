---
title: "GanttChartView.TableTextStyles"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GanttChartView. Λαμβάνει μια λίστα των στυλ κειμένου πίνακα της προβολής Gantt Chart. TableTextStyle"
type: docs
weight: 160
url: /el/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Λαμβάνει μια λίστα των στυλ κειμένου πίνακα της προβολής Gantt Chart. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε προσαρμοσμένα στυλ κειμένου πίνακα.

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

### Δείτε επίσης

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


