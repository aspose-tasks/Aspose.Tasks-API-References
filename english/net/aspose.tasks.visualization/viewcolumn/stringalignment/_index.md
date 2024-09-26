---
title: ViewColumn.StringAlignment
second_title: Aspose.Tasks for .NET API Reference
description: ViewColumn property. Gets or sets alignment of the text can be one of the values of the HorizontalStringAlignment enumeration
type: docs
weight: 30
url: /net/aspose.tasks.visualization/viewcolumn/stringalignment/
---
## ViewColumn.StringAlignment property

Gets or sets alignment of the text (can be one of the values of the [`HorizontalStringAlignment`](../../horizontalstringalignment/) enumeration).

```csharp
public HorizontalStringAlignment StringAlignment { get; set; }
```

## Examples

Shows how to set a alignment of the text in a column (can be one of the values of the &lt;see cref="P:Aspose.Tasks.Visualization.ViewColumn.StringAlignment" /&gt; enumeration).

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions();
options.Timescale = Timescale.Months;
options.View = ProjectView.GetDefaultGanttChartView();

var column1 = (GanttChartColumn)options.View.Columns[2];
column1.StringAlignment = HorizontalStringAlignment.Center;
var column2 = (GanttChartColumn)options.View.Columns[3];
column2.StringAlignment = HorizontalStringAlignment.Far;
var column3 = (GanttChartColumn)options.View.Columns[4];
column3.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_GanttChart_out.pdf", options);

options.PresentationFormat = PresentationFormat.ResourceSheet;
options.View = ProjectView.GetDefaultResourceSheetView();

var column4 = (ResourceViewColumn)options.View.Columns[2];
column4.StringAlignment = HorizontalStringAlignment.Center;
var column5 = (ResourceViewColumn)options.View.Columns[3];
column5.StringAlignment = HorizontalStringAlignment.Far;
var column6 = (ResourceViewColumn)options.View.Columns[4];
column6.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_ResourceSheet_out.pdf", options);
```

### See Also

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


