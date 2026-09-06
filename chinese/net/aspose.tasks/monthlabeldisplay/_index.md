---
title: "枚举 MonthLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MonthLabelDisplay 枚举。指定月份标签的显示方式"
type: docs
weight: 1060
url: /zh/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

指定月份标签的显示方式。

```csharp
public enum MonthLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Mo | `0` | 将 MS Project 中的月份列表设置为 mo。 |
| Mon | `1` | 将 MS Project 中的月份列表设置为 mon。 |
| Month | `2` | 将 MS Project 中的月份列表设置为 month。 |

## 示例

展示如何设置项目显示选项的月份标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置月份标签的显示方式
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


