---
title: Struct Duration
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Duration 结构. 表示项目中的持续时间
type: docs
weight: 470
url: /zh/net/aspose.tasks/duration/
---
## Duration structure

表示项目中的持续时间。

```csharp
public struct Duration : IEquatable<Duration>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | 获取一个值，指示时间单位是否已过。 确定此 Duration 实例是否已过的标志。 |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | 获取时间单位是否估计的值。 确定是否估计此 Duration 实例的标志。 |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | 获取[`TimeSpan`](./timespan/)此 Duration 对象的实例. 此 Duration 对象的 TimeSpan 实例。 |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | 获取此对象的时间单位类型。 此 Duration 实例的时间单位类型。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | 将指定字符串转换为的实例`Duration`结构. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | 将指定的双精度值添加到此持续时间。 |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | 将指定的持续时间添加到此持续时间。 |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | 将 Duration 对象转换为具有指定时间单位的另一个持续时间。 |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | 返回一个值，指示此实例是否等于指定对象。 |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定对象。 |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | 返回此对象的哈希码值。 |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | 从此持续时间实例中减去指定的双精度值。 |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | 从此持续时间实例中减去指定的持续时间。 |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | 将 Duration 对象转换为Double值. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | 返回此实例的字符串表示。 |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | 解析格式为“PT--H--M--S--”的持续时间字符串。 |
| [operator ==](../../aspose.tasks/duration/op_equality/) | 返回一个值，指示此实例是否等于指定对象。 |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | 返回一个值，指示此实例是否不等于指定对象。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


