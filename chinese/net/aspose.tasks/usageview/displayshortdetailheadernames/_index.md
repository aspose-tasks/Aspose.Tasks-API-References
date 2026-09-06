---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Aspose.Tasks for .NET API 参考"
description: "UsageView 属性。获取或设置一个值，指示是否显示简短的详细标题名称"
type: docs
weight: 40
url: /zh/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

获取或设置一个值，指示是否显示简短的详细标题名称。

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
```

## 示例

展示如何渲染带有详细信息的任务使用视图。

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// 获取视图
UsageView view = (TaskUsageView)project.DefaultView;

// 详细标题列将不会显示
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// 显示详细标题列
view.DisplayDetailsHeaderColumn = true;

// 在所有分配行上重复详细标题
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


