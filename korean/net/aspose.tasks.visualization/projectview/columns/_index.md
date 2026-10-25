---
title: "ProjectView.Columns"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectView 속성. 프로젝트 보기 열을 가져옵니다"
type: docs
weight: 70
url: /ko/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

프로젝트 뷰 열을 가져옵니다.

```csharp
public List<ViewColumn> Columns { get; }
```

## 예제

사용자 정의 열 집합을 가진 보기를 사용하여 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// 보기 열을 반복합니다
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### 또 보기

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


