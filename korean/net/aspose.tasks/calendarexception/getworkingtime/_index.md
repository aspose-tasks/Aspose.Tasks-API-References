---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 메서드. 캘린더 예외에 대한 작업 시간을 반환합니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

캘린더 예외에 대한 작업 시간을 반환합니다.

```csharp
public TimeSpan GetWorkingTime()
```

### 반환 값

이 캘린더 예외에 대한 작업 시간을 반환합니다.

## 예제

캘린더 예외의 작업 시간을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### 또 보기

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


