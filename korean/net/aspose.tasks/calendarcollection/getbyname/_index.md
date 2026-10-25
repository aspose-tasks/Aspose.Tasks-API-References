---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. 지정된 이름을 가진 캘린더를 반환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

지정된 이름을 가진 캘린더를 반환합니다.

```csharp
public Calendar GetByName(string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 캘린더의 이름. |

### 반환 값

찾은 경우 지정된 이름의 캘린더를 반환하고, 그렇지 않으면 null을 반환합니다.

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


