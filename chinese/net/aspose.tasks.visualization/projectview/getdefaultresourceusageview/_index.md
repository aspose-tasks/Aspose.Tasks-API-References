---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 方法。包括 Uid、名称、开始、完成和工作资源列"
type: docs
weight: 50
url: /zh/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

包括 Uid、名称、开始、完成和工作资源列。

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### 返回值

一个包含 [`ResourceViewColumn`](../../resourceviewcolumn/) 列表的视图。

## 示例

展示如何使用资源使用视图保存项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### 另见

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


