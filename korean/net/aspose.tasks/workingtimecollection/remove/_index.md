---
title: "WorkingTimeCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkingTimeCollection 메서드. 이 컬렉션에서 WorkingTime 인스턴스를 제거합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/workingtimecollection/remove/
---
## WorkingTimeCollection.Remove method

이 컬렉션에서 [`WorkingTime`](../../workingtime/) 인스턴스를 제거합니다.

```csharp
public bool Remove(WorkingTime item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | WorkingTime | 제거할 항목입니다. |

### 반환 값

이 컬렉션에서 WorkingTime 인스턴스가 성공적으로 제거된 경우 true; 그렇지 않으면 false.

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

* class [WorkingTime](../../workingtime/)
* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


