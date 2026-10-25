---
title: "Project.Views"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 View 对象的列表"
type: docs
weight: 1020
url: /zh/net/aspose.tasks/project/views/
---
## Project.Views property

获取一个 [`View`](../../view/) 对象的列表。

```csharp
public ViewCollection Views { get; }
```

## 示例

展示如何设置默认项目视图。

```csharp
var project = new Project(DataDir + "Project5.mpp");

View view = null;
foreach (var v in project.Views)
{
    if (v.Name == "&Gantt Chart")
    {
        view = v;
    }
}

// 设置默认视图
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### 另见

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


