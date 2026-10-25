---
title: "ViewColumn.StringAlignment"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ViewColumn. تحصل أو تعين محاذاة النص ويمكن أن تكون واحدة من قيم تعداد HorizontalStringAlignment."
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/viewcolumn/stringalignment/
---
## ViewColumn.StringAlignment property

يحصل أو يعين محاذاة النص (يمكن أن تكون واحدة من قيم تعداد [`HorizontalStringAlignment`](../../horizontalstringalignment/)).

```csharp
public HorizontalStringAlignment StringAlignment { get; set; }
```

## الأمثلة

يوضح كيفية تعيين محاذاة النص في عمود (يمكن أن تكون إحدى قيم تعداد <see cref="P:Aspose.Tasks.Visualization.ViewColumn.StringAlignment" />).

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

### انظر أيضًا

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


