---
title: Class WeekDay
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.WeekDay 班级. 表示一个工作日它定义了一周中的常规日期或日历中的例外日期
type: docs
weight: 3180
url: /zh/net/aspose.tasks/weekday/
---
## WeekDay class

表示一个工作日，它定义了一周中的常规日期或日历中的例外日期。

```csharp
public class WeekDay
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [WeekDay](weekday/#constructor)() | 初始化一个新的实例`WeekDay`类. |
| [WeekDay](weekday/#constructor_1)(DayType) | 初始化一个新的实例`WeekDay`具有指定日期类型的类。 |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | 初始化一个新的实例`WeekDay`具有指定日期类型和工作时间段列表的类。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | 获取一天的类型。 |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | 获取或设置一个值，该值指示指定的日期或日期类型是否有效。 |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | 获取或设置异常时间的开始。 |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | 获取或设置异常结束时间。 |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | 获取此 WeekDay 实例的 WorkingTimeCollection。 定义工作日工作时间的工作时间集合。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | 创建默认工作日。 |
| [Clone](../../aspose.tasks/weekday/clone/)() | 返回工作日的深拷贝。 |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | 返回一个值，指示此实例是否等于指定对象。 |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | 返回实例的哈希码值`WeekDay`类. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | 返回工作日的工作时间。 |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | 转换 .Net 的DayOfWeek到[`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | 设置指定工作日的默认时间段。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


