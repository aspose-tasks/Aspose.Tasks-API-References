---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageMargins 属性。获取或设置打印边框的位置。可以是 Border 枚举的其中一个值"
type: docs
weight: 20
url: /zh/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

获取或设置打印边框的位置。可以是[`Border`](../../border/)枚举的其中一个值。

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


