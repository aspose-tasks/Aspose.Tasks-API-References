---
title: WorkingTime.WorkingTime
second_title: Aspose.Tasks for .NET API 参考
description: WorkingTime 构造函数. 初始化一个新的实例WorkingTime以指定的开始和结束时间间隔上课
type: docs
weight: 10
url: /zh/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

初始化一个新的实例[`WorkingTime`](../)以指定的开始和结束时间间隔上课。

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fromTime | DateTime | 间隔开始时间 |
| toTime | DateTime | 间隔结束时间 |

### 也可以看看

* class [WorkingTime](../)
* 命名空间 [Aspose.Tasks](../../workingtime/)
* 部件 [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

初始化一个新的实例[`WorkingTime`](../)具有指定开始和结束时间的间隔项的类。

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fromTime | TimeSpan | Interval 的开始时间表示为TimeSpan结构。 |
| toTime | TimeSpan | Interval 的结束时间表示为TimeSpan结构。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | 当 toTime 小于或等于 toTime argument 或当 fromTime 和 toTime 之间的间隔大于 24 小时时。 |

### 例子

WorkingTime ctor 的重载可用于使用 TimeSpans: 初始化间隔的开始和结束

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### 也可以看看

* class [WorkingTime](../)
* 命名空间 [Aspose.Tasks](../../workingtime/)
* 部件 [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

初始化一个新的实例[`WorkingTime`](../)具有指定开始和结束时间的间隔项的类。

```csharp
public WorkingTime(int fromHours, int toHours)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fromHours | Int32 | 间隔的开始时间以小时数 (0-24) 表示。 |
| toHours | Int32 | 间隔的结束时间以小时数 (0-24) 表示。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | 当 toTime 小于或等于 toTime argument 或当 fromTime 和 toTime 之间的间隔大于 24 小时时。 |

### 例子

WorkingTime ctor 的重载可用于使用整小时初始化间隔的开始和结束：

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### 也可以看看

* class [WorkingTime](../)
* 命名空间 [Aspose.Tasks](../../workingtime/)
* 部件 [Aspose.Tasks](../../../)


