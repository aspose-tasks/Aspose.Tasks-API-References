---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 이 객체에 대한 DayTypeCollection을 가져옵니다. 예외가 유효한 요일을 나타냅니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

이 객체에 대한 DayTypeCollection을 가져옵니다. 예외가 유효한 요일입니다.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## 예제

요일별로 캘린더 예외를 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 캘린더를 생성합니다.
var calendar = project.Calendars.Add("Calendar1");

// 매 금요일에 대한 캘린더 예외를 생성합니다.
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// 금요일이 예외인지 확인합니다.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// 예외를 캘린더에 추가합니다
calendar.Exceptions.Add(exception);
```

### 또 보기

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


