---
title: "클래스 CalendarExceptionCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalendarExceptionCollection 클래스. CalendarException 객체의 컬렉션을 나타냅니다"
type: docs
weight: 260
url: /ko/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

[`CalendarException`](../calendarexception/) 객체의 컬렉션을 나타냅니다.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | `CalendarExceptionCollection` 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | 이 객체의 상위 캘린더를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | CalendarException 인스턴스를 이 컬렉션 객체에 추가합니다. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | 예외 범위를 내부 목록에 추가합니다. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | `CalendarExceptionCollection`에서 모든 항목을 제거합니다. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | 이 컬렉션에서 [`CalendarException`](../calendarexception/) 인스턴스를 제거합니다. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | CalendarExceptionCollection 객체를 [`CalendarException`](../calendarexception/) 객체 목록으로 변환합니다. |

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

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


