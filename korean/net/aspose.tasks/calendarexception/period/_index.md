---
title: "CalendarException.Period"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 예외에 대한 반복 기간을 가져오거나 설정합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/calendarexception/period/
---
## CalendarException.Period property

예외의 반복 기간을 가져오거나 설정합니다.

```csharp
public int Period { get; set; }
```

## 예제

월 일별로 캘린더 예외를 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 캘린더를 생성합니다.
var calendar = project.Calendars.Add("Calendar1");

// 매 금요일에 대한 캘린더 예외를 생성합니다.
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// aa 금요일이 예외인지 확인합니다.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// 예외를 캘린더에 추가합니다
calendar.Exceptions.Add(exception);
```

### 또 보기

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


