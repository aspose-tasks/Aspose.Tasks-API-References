---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。根据日历计算在指定工作时间量过去后对应的日期"
type: docs
weight: 160
url: /zh/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

根据日历计算指定工作时间量过去后的日期。

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 开始日期。 |
| 工作 | 持续时间 | 工作持续时间。 |

### 返回值

结束日期。

## 示例

展示如何使用日历实例通过开始日期和工作量计算完成日期。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// 使用标准日历计算完成日期
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### 另见

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

根据日历计算指定工作时间量过去后的日期。

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 开始日期。 |
| 工作 | TimeSpan | 工作持续时间。 |

### 返回值

结束日期。

## 示例

展示如何使用日历实例通过开始日期和工作（作为时间跨度）计算完成日期。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// 使用标准日历计算完成日期
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


