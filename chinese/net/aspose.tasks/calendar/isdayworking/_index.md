---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。确定指定日期是否为工作日（根据日历）"
type: docs
weight: 260
url: /zh/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

确定指定日期是否为日历中的工作日。

```csharp
public bool IsDayWorking(DateTime dt)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | DateTime | 用于检查该日是否为工作日的日期。 |

### 返回值

如果该日是工作日，则为 True。

## 示例

展示如何计算工作小时。

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// 通过 Id 访问任务
var task = project.RootTask.Children.GetById(1);

// 访问日历及其开始和结束日期
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// 访问资源及其日历
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// 获取分钟为单位的持续时间
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// 获取小时为单位的持续时间
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// 获取天为单位的持续时间
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


