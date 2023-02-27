---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks for .NET API 参考
description: TaskLink 财产. 获取或设置滞后持续时间具体取决于 LagFormat.
type: docs
weight: 50
url: /zh/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

获取或设置滞后持续时间，具体取决于 LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | 尝试设置 LagFormat 为 TimeUnitType.Percent 的 TaskLinks 的值时。 |

### 评论

链接延迟可以是百分比值（LagFormat 是 TimeUnitType.Percent）。 在这种情况下，持续时间计算为 PredTask 持续时间的百分比。 否则，该方法返回表示 TaskLink 延迟的 TimeSpan 值。

### 也可以看看

* class [TaskLink](../)
* 命名空间 [Aspose.Tasks](../../tasklink/)
* 部件 [Aspose.Tasks](../../../)


