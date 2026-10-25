---
title: "ViewColumn.StringAlignment"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ViewColumn 속성. 텍스트 정렬을 가져오거나 설정합니다. 정렬은 HorizontalStringAlignment 열거형의 값 중 하나일 수 있습니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/viewcolumn/stringalignment/
---
## ViewColumn.StringAlignment property

텍스트 정렬을 가져오거나 설정합니다(값은 [`HorizontalStringAlignment`](../../horizontalstringalignment/) 열거형 중 하나일 수 있습니다).

```csharp
public HorizontalStringAlignment StringAlignment { get; set; }
```

## 예제

열에 텍스트 정렬을 설정하는 방법을 보여줍니다 (열 정렬은 &lt;see cref="P:Aspose.Tasks.Visualization.ViewColumn.StringAlignment" /&gt; 열거형의 값 중 하나일 수 있습니다).

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

### 또 보기

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


