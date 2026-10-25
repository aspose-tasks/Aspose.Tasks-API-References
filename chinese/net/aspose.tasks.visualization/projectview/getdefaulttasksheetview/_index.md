---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 方法。包括 id、指示符、名称、持续时间、开始、完成、前置任务和资源名称任务列"
type: docs
weight: 60
url: /zh/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

包括 id、指示器、名称、持续时间、开始、完成、前置任务和资源名称任务列。

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### 返回值

一个视图，其中包含 [`GanttChartColumn`](../../ganttchartcolumn/) 列表。

## 示例

展示如何使用任务表视图保存项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### 另见

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


