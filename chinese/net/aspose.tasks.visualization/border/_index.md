---
title: "枚举 Border"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.Border 枚举。指定边框类型。"
type: docs
weight: 2970
url: /zh/net/aspose.tasks.visualization/border/
---
## Border enumeration

指定类型边框。

```csharp
public enum Border
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| NoBorder | `0` | 无边框。 |
| AroundEveryPage | `1` | 每页周围。 |
| OutsidePages | `2` | 在外部页面上。 |

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


