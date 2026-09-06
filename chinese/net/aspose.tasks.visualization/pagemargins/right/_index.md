---
title: "PageMargins.Right"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageMargins 属性。获取或设置右侧边距的大小（单位：厘米）。"
type: docs
weight: 50
url: /zh/net/aspose.tasks.visualization/pagemargins/right/
---
## PageMargins.Right property

获取或设置右侧边距的大小（单位：厘米）。

```csharp
public double Right { get; set; }
```

## 示例

展示如何使用页面边距。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 让我们修改默认视图
var margins = project.DefaultView.PageInfo.Margins;

// 让我们修改边距
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


