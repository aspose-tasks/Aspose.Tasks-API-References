---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CsvOptions 속성. XLSX 형식으로 저장하기 위한 보기 열 GanttChartColumn 목록을 가져오거나 설정합니다. 설정하지 않으면 기본 열이 저장됩니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

XLSX 형식으로 저장하기 위한 보기 열 ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) 목록을 가져오거나 설정합니다. 설정하지 않으면 기본 열이 저장됩니다.

```csharp
public ProjectView View { get; set; }
```

## 예제

기본 Gantt 차트의 열을 가져오기 위해 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt;을 사용하는 방법을 보여줍니다.

```csharp
// CSV 파일에 저장합니다.
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

### 또 보기

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


