---
title: "枚举 HourLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.HourLabelDisplay 枚举。指定小时标签的显示方式。"
type: docs
weight: 820
url: /zh/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

指定小时标签的显示方式。

```csharp
public enum HourLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| H | `0` | “h” 标签。 |
| Hr | `1` | “hr” 标签。 |
| Hour | `2` | “hour(s)” 标签。 |

## 示例

展示如何设置项目显示选项的小时标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置小时标签的显示方式
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


