---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。根据指定的结束日期和持续时间返回开始日期"
type: docs
weight: 200
url: /zh/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

根据指定的结束日期和持续时间返回开始日期。

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 结束 | DateTime | 指定的结束日期。 |
| 持续时间 | 持续时间 | 指定的持续时间。 |

### 返回值

计算得到的开始日期。

## 示例

展示如何通过结束日期和持续时间获取开始日期。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 通过结束日期和持续时间获取开始日期
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 2020年4月8日 上午9:00 将被打印
Console.WriteLine(startDate);
```

### 另见

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

根据指定的结束日期和持续时间返回开始日期。

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 结束 | DateTime | 指定的结束日期。 |
| 持续时间 | TimeSpan | 指定的持续时间。 |

### 返回值

计算得到的开始日期。

## 示例

展示如何通过结束日期和持续时间（作为时间跨度）获取开始日期。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 通过结束日期和持续时间获取开始日期
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 2020年4月8日 上午9:00 将被打印
Console.WriteLine(startDate);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


