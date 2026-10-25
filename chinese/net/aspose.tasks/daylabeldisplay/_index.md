---
title: "枚举 DayLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DayLabelDisplay 枚举。指定天标签的显示方式"
type: docs
weight: 440
url: /zh/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

指定日期标签的显示方式。

```csharp
public enum DayLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| D | `0` | 将 MS Project 中的 Days 列表设置为 d。 |
| Dy | `1` | 将 MS Project 中的 Days 列表设置为 dy。 |
| Day | `2` | 将 MS Project 中的 Days 列表设置为 day。 |

## 示例

展示如何设置项目显示选项的天标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置日期标签的显示方式
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


