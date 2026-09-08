---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. CalendarCollection 객체를 Calendar 객체 목록으로 변환합니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

CalendarCollection 객체를 [`Calendar`](../../calendar/) 객체 목록으로 변환합니다.

```csharp
public List<Calendar> ToList()
```

### 반환 값

`[`Calendar`](../../calendar/)` 객체 목록.

## 예제

캘린더 컬렉션을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


