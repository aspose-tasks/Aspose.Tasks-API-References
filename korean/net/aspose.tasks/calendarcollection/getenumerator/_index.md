---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. 이 컬렉션에 대한 열거자를 반환합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

이 컬렉션에 대한 열거자를 반환합니다.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### 반환 값

이 컬렉션에 대한 열거자.

## 예제

새 캘린더를 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 캘린더는 컬렉션의 Add 오버로드를 사용하여 프로젝트의 캘린더 컬렉션에 추가할 수 있습니다.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


