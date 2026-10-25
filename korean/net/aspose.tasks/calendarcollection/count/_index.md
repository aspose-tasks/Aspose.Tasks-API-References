---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 속성. 이 CalendarCollection 객체에 포함된 객체 수를 가져옵니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

이 [`CalendarCollection`](../) 객체에 포함된 객체 수를 가져옵니다.

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


