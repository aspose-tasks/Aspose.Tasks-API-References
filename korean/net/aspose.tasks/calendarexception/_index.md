---
title: "클래스 CalendarException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalendarException 클래스. 캘린더에서 예외적인 시간 기간을 나타냅니다"
type: docs
weight: 250
url: /ko/net/aspose.tasks/calendarexception/
---
## CalendarException class

캘린더의 예외적인 시간 기간을 나타냅니다.

```csharp
public sealed class CalendarException
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CalendarException](calendarexception/)() | 새 `CalendarException` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | 이 객체에 대한 DayTypeCollection을 가져옵니다. 예외가 유효한 요일입니다. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | 지정된 날짜 또는 day type이 작업일인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 가져오거나 설정합니다. False는 반복 범위가 종료 날짜 입력으로 정의된다는 것을 지정합니다. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | 예외 시간의 시작을 가져오거나 설정합니다. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | 예외 반복이 예정된 월을 가져오거나 설정합니다. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | 예외 반복이 예정된 월의 일을 가져오거나 설정합니다. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | 예외 반복이 예정된 월 항목을 가져오거나 설정합니다. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | 월 내에서 월 항목의 위치를 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | 예외의 이름을 가져오거나 설정합니다. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | 캘린더 예외가 유효한 발생 횟수를 가져오거나 설정합니다. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | 이 객체의 상위 캘린더를 가져옵니다. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | 예외의 반복 기간을 가져오거나 설정합니다. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | 예외 시간의 종료를 가져오거나 설정합니다. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | 예외 유형을 가져오거나 설정합니다. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | WorkingTimeCollection 객체를 가져오거나 설정합니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다. 최소 하나의 작업 시간이 존재해야 하며, 다섯 개를 초과할 수 없습니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | 지정된 DateTime 구조체 인스턴스가 예외일인 경우 true를 반환합니다. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | 부모 캘린더인 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | 캘린더 예외가 적용되는 날짜들을 반환합니다. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | 캘린더 예외에 대한 작업 시간을 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


