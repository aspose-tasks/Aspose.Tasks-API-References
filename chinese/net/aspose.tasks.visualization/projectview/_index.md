---
title: "类 ProjectView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.ProjectView 类。项目视图类"
type: docs
weight: 3300
url: /zh/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

项目视图类

```csharp
public class ProjectView
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | 初始化 `ProjectView` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | 获取项目视图列。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | 包括 Uid、任务名称、资源名称、工作和持续时间分配列。 |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | 包括 id、指示器、名称、持续时间、开始和完成任务列。 |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | 包括 Uid、资源名称、类型、材料标签、缩写、组、最大单位、标准费率、加班费率、每次使用费用、累计时间、基础日历和代码资源列。 |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | 包括 Uid、名称、开始、完成和工作资源列。 |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | 包括 id、指示器、名称、持续时间、开始、完成、前置任务和资源名称任务列。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


