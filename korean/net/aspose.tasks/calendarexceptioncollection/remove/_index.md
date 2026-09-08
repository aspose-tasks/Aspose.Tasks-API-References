---
title: "CalendarExceptionCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarExceptionCollection 메서드. 이 컬렉션에서 CalendarException 인스턴스를 제거합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/calendarexceptioncollection/remove/
---
## CalendarExceptionCollection.Remove method

이 컬렉션에서 [`CalendarException`](../../calendarexception/) 인스턴스를 제거합니다.

```csharp
public bool Remove(CalendarException item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | CalendarException | 제거할 항목입니다. |

### 반환 값

지정된 예외가 성공적으로 제거되면 true.

## 예제

캘린더 예외를 정의하기 위해 캘린더 예외 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// 모든 예외를 제거합니다
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### 또 보기

* class [CalendarException](../../calendarexception/)
* class [CalendarExceptionCollection](../)
* namespace [Aspose.Tasks](../../calendarexceptioncollection/)
* assembly [Aspose.Tasks](../../../)


