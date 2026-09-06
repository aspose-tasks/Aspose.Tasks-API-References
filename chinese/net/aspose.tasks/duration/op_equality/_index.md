---
title: "Duration.op_Equality"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。返回一个值，指示此实例是否等于指定的对象。"
type: docs
weight: 140
url: /zh/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

返回一个值，指示此实例是否等于指定的对象。

```csharp
public static bool operator ==(Duration a, Duration b)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | 持续时间 | 第一个 Duration。 |
| b | 持续时间 | 第二个 Duration。 |

### 返回值

一个指示此实例是否等于指定对象的值。

## 示例

展示如何检查 Duration 相等性。

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// Duration 的相等性是相对于底层 TimeSpan 进行检查的。
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


