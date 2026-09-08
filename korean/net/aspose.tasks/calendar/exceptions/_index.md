---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. CalendarExceptionCollection 객체를 가져옵니다. 캘린더와 연결된 예외 컬렉션입니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

CalendarExceptionCollection 객체를 가져옵니다. 캘린더와 연결된 예외 컬렉션입니다.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## 예제

캘린더 예외에 대한 정보를 검색하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// 캘린더를 반복합니다
foreach (var calendar in project.Calendars)
{
    // 캘린더 예외에 접근하기
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### 또 보기

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


