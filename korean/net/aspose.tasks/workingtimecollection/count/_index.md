---
title: "WorkingTimeCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkingTimeCollection 속성. 이 WorkingTimeCollection 객체에 포함된 객체 수를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/workingtimecollection/count/
---
## WorkingTimeCollection.Count property

이 [`WorkingTimeCollection`](../) 객체에 포함된 객체 수를 가져옵니다.

```csharp
public int Count { get; }
```

## 예제

작업 시간 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// Saturday의 작업 시간을 출력합니다
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// sunday의 작업 시간을 출력합니다
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // 작업 시간을 추가로 탐색하고 이를 표시할 수 있습니다.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### 또 보기

* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


