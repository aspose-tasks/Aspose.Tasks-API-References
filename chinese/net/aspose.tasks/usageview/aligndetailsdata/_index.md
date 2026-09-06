---
title: "UsageView.AlignDetailsData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "UsageView 属性。获取或设置详细数据的对齐方式"
type: docs
weight: 10
url: /zh/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

获取或设置详细数据对齐方式。

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


