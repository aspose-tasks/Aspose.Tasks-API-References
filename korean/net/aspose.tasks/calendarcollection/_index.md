---
title: "클래스 CalendarCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalendarCollection 클래스. Calendar 객체의 컬렉션을 나타냅니다"
type: docs
weight: 240
url: /ko/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

[`Calendar`](../calendar/) 객체의 컬렉션을 나타냅니다.

```csharp
public class CalendarCollection : IList<Calendar>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | `CalendarCollection` 객체에 포함된 객체 수를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | 이 CalendarCollection 객체에 새 기본 캘린더를 추가하고 추가된 캘린더를 반환합니다. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | 지정된 기본 캘린더와 함께 새 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | 지정된 이름을 가진 캘린더를 반환합니다. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | 지정된 UID를 가진 캘린더를 반환합니다. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | 프로젝트 CalendarCollection에서 캘린더를 제거합니다. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | CalendarCollection 객체를 [`Calendar`](../calendar/) 객체 목록으로 변환합니다. |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


