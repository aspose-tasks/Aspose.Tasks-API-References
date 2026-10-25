---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. 지정된 UID를 가진 캘린더를 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

지정된 UID를 가진 캘린더를 반환합니다.

```csharp
public Calendar GetByUid(int uid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | Int32 | 캘린더의 UID. |

### 반환 값

지정된 UID를 가진 캘린더.

## 예제

이름 또는 ID로 캘린더를 가져오는 방법을 보여줍니다

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


