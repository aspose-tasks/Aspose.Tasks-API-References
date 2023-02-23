---
title: Class TimephasedData
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.TimephasedData 班级. 表示一个时间分段数据
type: docs
weight: 2280
url: /zh/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

表示一个时间分段数据。

```csharp
public class TimephasedData
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TimephasedData](timephaseddata/)() | 初始化一个新的实例`TimephasedData`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | 获取或设置时间分段数据周期的结束日期。 |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | 获取或设置时间分段数据周期的开始日期。 |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | 获取或设置时间分段数据的类型。 |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | 获取或设置时间分段数据的唯一标识符 |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | 获取或设置时间分段数据周期的时间单位。 |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | 获取或设置时间分段数据周期的每单位时间值。 |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; } | 获取Double表示此对象的字符串值的实例. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | 获取TimeSpan表示此对象的字符串值的实例. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | 获取Double表示基于单位的时间分段数据的此对象的字符串值的实例。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | 创建并初始化一个新的实例`TimephasedData`基于成本的时间分段数据类. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | 创建并初始化一个新的实例`TimephasedData`材料资源分配的基于单位的时间分段数据的类。 |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | 创建并初始化一个新的实例`TimephasedData`基于工作的时间分段数据类. |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


