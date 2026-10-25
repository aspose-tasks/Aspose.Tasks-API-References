---
title: "CalendarException.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 예외의 이름을 가져오거나 설정합니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/calendarexception/name/
---
## CalendarException.Name property

예외의 이름을 가져오거나 설정합니다.

```csharp
public string Name { get; set; }
```

## 예제

캘린더 예외를 추가/제거하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 캘린더를 생성합니다.
var calendar = project.Calendars.Add("Calendar1");

// 휴일에 대한 주중 예외를 생성합니다.
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// 해당 날짜가 예외인지 확인합니다.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// 예외를 제거합니다.
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// 예외를 추가합니다.
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// 예외를 출력합니다.
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### 또 보기

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


