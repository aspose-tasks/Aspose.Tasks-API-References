---
title: CsvOptions.View
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions property. Gets or sets a list of the view columns GanttChartColumn to save to XLSX format. If not set then default columns are saved
type: docs
weight: 60
url: /net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Gets or sets a list of the view columns ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) to save to XLSX format. If not set then default columns are saved.

```csharp
public ProjectView View { get; set; }
```

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; to take the columns of the default Gantt Chart and

```csharp
// save them to a CSV file.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### See Also

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


