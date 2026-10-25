---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectView 方法。包括 Uid、资源名称、类型、材料、标签、首字母、组、最大单位、标准费率、加班费率、每次使用成本、累计于基础日历以及代码资源列"
type: docs
weight: 40
url: /zh/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

包括 Uid、资源名称、类型、材料标签、缩写、组、最大单位、标准费率、加班费率、每次使用费用、累计时间、基础日历和代码资源列。

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### 返回值

一个包含 [`ResourceViewColumn`](../../resourceviewcolumn/) 列表的视图。

## 示例

展示如何使用资源表视图保存项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### 另见

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


