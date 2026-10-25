---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 方法。包括 id、指示符、名称、持续时间、开始和完成任务列"
type: docs
weight: 30
url: /zh/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

包括 id、指示器、名称、持续时间、开始和完成任务列。

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### 返回值

一个视图，其中包含 [`GanttChartColumn`](../../ganttchartcolumn/) 列表。

## 示例

展示如何使用甘特图视图保存项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### 另见

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


