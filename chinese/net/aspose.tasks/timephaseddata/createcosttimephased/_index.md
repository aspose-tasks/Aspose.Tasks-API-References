---
title: TimephasedData.CreateCostTimephased
second_title: Aspose.Tasks for .NET API 参考
description: TimephasedData 方法. 创建并初始化一个新的实例TimephasedData基于成本的时间分段数据类.
type: docs
weight: 20
url: /zh/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

创建并初始化一个新的实例[`TimephasedData`](../)基于成本的时间分段数据类.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| uid | Int32 | 任务的 UID。 |
| start | DateTime | 开始日期时间。 |
| finish | DateTime | 完成日期时间。 |
| value | Double | 成本价值。 |
| timeUnit | TimeUnitType | 时间单位类型。 |
| type | TimephasedDataType | 时间分段数据类型。 |

### 返回值

的一个实例[`TimephasedData`](../)基于成本的时间分段数据的类。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | 如果指定了负成本值。 |

### 也可以看看

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* 命名空间 [Aspose.Tasks](../../timephaseddata/)
* 部件 [Aspose.Tasks](../../../)


