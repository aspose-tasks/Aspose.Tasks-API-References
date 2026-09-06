---
title: "枚举 WeekLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeekLabelDisplay 枚举。指定周标签的显示方式"
type: docs
weight: 3560
url: /zh/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

指定周标签的显示方式。

```csharp
public enum WeekLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| W | `0` | "w" 标签。 |
| Wk | `1` | "wk" 标签。 |
| Week | `2` | "week" 标签。 |

## 示例

展示如何设置项目显示选项的周标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置周标签的显示方式
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


