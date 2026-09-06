---
title: "类 PageMargins"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.PageMargins 类。表示用于打印的页面边距。"
type: docs
weight: 3230
url: /zh/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

表示用于打印的页面边距。

```csharp
public class PageMargins
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PageMargins](pagemargins/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | 获取或设置打印边框的位置。可以是 [`Border`](../border/) 枚举的其中一个值。 |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | 获取或设置底部边距的大小（单位：厘米）。 |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | 获取或设置左侧边距的大小（单位：厘米）。 |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | 获取或设置右侧边距的大小（单位：厘米）。 |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | 获取或设置顶部边距的大小（单位：厘米）。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


