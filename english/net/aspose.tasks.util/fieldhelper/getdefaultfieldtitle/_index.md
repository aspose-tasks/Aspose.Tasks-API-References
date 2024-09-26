---
title: FieldHelper.GetDefaultFieldTitle
second_title: Aspose.Tasks for .NET API Reference
description: FieldHelper method. Returns a default title of the specific field
type: docs
weight: 10
url: /net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Returns a default title of the specific field.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parameter | Type | Description |
| --- | --- | --- |
| field | Field | Field to get a default title. |

### Return Value

A default title of the specific field if the field can be displayed in MS Project's view, null otherwise.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


