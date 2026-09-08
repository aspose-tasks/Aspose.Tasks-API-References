---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 메서드. 상위 캘린더 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다."
type: docs
weight: 180
url: /ko/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

부모 캘린더인 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다.

```csharp
public void Delete()
```

## 예제

캘린더 예외를 삭제하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// 예외를 제거합니다.
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### 또 보기

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


