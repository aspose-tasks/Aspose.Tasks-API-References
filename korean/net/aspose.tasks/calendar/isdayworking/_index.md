---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 날짜가 캘린더에 따라 작업일인지 여부를 판단합니다."
type: docs
weight: 260
url: /ko/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

캘린더에 따라 지정된 날짜가 작업일인지 여부를 판단합니다.

```csharp
public bool IsDayWorking(DateTime dt)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | DateTime | 해당 날짜가 근무일인지 확인하기 위한 날짜. |

### 반환 값

날짜가 근무일이면 True.

## 예제

작업 시간을 계산하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// ID로 작업에 접근합니다.
var task = project.RootTask.Children.GetById(1);

// Calendar와 그 시작 및 종료 날짜에 접근합니다.
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// 리소스와 해당 캘린더에 접근합니다.
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// 분 단위 지속 시간 가져오기
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

// 시간 단위 지속 시간 가져오기
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

// 일 단위 지속 시간 가져오기
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

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


