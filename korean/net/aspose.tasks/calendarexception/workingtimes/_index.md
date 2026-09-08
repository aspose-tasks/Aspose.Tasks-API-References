---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. WorkingTimeCollection 객체를 가져오거나 설정합니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다. 최소 하나의 작업 시간이 존재해야 하며, 다섯 개를 초과할 수 없습니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

WorkingTimeCollection 객체를 가져오거나 설정합니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다. 최소 하나의 작업 시간이 존재해야 하며, 다섯 개를 초과할 수 없습니다.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


