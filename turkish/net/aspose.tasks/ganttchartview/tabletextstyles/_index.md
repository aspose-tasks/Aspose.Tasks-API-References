---
title: "GanttChartView.TableTextStyles"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Şeması görünümünün tablo metin stillerinin bir listesini alır. TableTextStyle"
type: docs
weight: 160
url: /tr/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Gantt Şeması görünümünün tablo metin stillerinin bir listesini alır. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## Örnekler

Özel tablo metin stillerinin nasıl ekleneceğini gösterir.

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

### Ayrıca Bakınız

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


