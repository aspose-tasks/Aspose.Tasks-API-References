---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 方法。包括 Uid、任务名称、资源名称、工作和持续时间分配列"
type: docs
weight: 20
url: /zh/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

包括 Uid、任务名称、资源名称、工作和持续时间分配列。

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### 返回值

一个包含 [`AssignmentViewColumn`](../../assignmentviewcolumn/) 列表的视图。

## 示例

展示如何使用分配视图保存项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### 另见

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


