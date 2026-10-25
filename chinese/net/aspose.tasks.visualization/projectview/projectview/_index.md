---
title: "ProjectView.ProjectView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 构造函数。初始化 ProjectView 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

初始化 [`ProjectView`](../) 类的新实例。

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | IEnumerable`1 | 视图列的列表。 |

## 示例

展示如何使用自定义列集合的视图保存项目。

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

// 遍历视图列
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### 另见

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


