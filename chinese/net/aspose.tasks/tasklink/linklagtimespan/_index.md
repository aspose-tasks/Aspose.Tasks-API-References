---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskLink 属性。获取或设置根据 LagFormat 的延迟持续时间"
type: docs
weight: 50
url: /zh/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

获取或设置延迟持续时间，取决于 LagFormat。

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当尝试为 LagFormat 为 TimeUnitType.Percent 的 TaskLinks 设置值时。 |

## 备注

链接延迟可以是百分比值（LagFormat 为 TimeUnitType.Percent）。在这种情况下，持续时间按 PredTask 持续时间的百分比计算。否则，该方法返回表示 TaskLink 延迟的 TimeSpan 值。

### 另见

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


