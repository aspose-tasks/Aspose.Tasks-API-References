---
title: Class CsvOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.CsvOptions class. Allows to specify additional options when saving project to CSV
type: docs
weight: 1960
url: /net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Allows to specify additional options when saving project to CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [CsvOptions](csvoptions/)() | Initializes a new instance of the `CsvOptions` class which can be used to save project in CSV format. |

## Properties

| Name | Description |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Gets or sets a data category to be saved. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Gets or sets an encoding to save CSV with. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Gets or sets a value indicating whether to include headers or not (default value is TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Gets or sets a text delimiter. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Gets or sets a list of the view columns ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) to save to XLSX format. If not set then default columns are saved. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; to save a project as CSV file.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


