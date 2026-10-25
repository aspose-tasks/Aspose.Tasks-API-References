---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 메서드. 캘린더 예외가 적용되는 날짜를 반환합니다"
type: docs
weight: 190
url: /ko/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

캘린더 예외가 적용되는 날짜들을 반환합니다.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### 반환 값

캘린더 예외가 적용되는 예외 날짜들의 컬렉션을 반환합니다

## 예제

특정 캘린더 예외가 유효한 날짜를 가져오는 방법을 보여줍니다

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### 또 보기

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


