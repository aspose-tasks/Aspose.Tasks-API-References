---
title: "枚举 YearLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.YearLabelDisplay 枚举。指定年份标签的显示方式"
type: docs
weight: 3680
url: /zh/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

指定年份标签的显示方式。

```csharp
public enum YearLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Y | `0` | 将 MS Project 中的 Years 列表设置为 mo。 |
| Yr | `1` | 将 MS Project 中的 Years 列表设置为 mon。 |
| Year | `2` | 将 MS Project 中的 Years 列表设置为月份。 |

## 示例

展示如何设置项目显示选项的年份标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置年份标签的显示方式
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


