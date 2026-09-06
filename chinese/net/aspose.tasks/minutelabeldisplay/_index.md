---
title: "枚举 MinuteLabelDisplay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MinuteLabelDisplay 枚举。指定分钟标签的显示方式。"
type: docs
weight: 1030
url: /zh/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

指定分钟标签的显示方式。

```csharp
public enum MinuteLabelDisplay
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| M | `0` | 将 MS Project 中的 Minutes 列表设置为 m。 |
| Min | `1` | 将 MS Project 中的 Minutes 列表设置为 min。 |
| Minute | `2` | 将 MS Project 中的 Minutes 列表设置为 minute。 |

## 示例

展示如何设置项目显示选项的分钟标签（案例 1）。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 设置分钟标签的显示方式
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


