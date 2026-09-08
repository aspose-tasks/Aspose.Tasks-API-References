---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarCollection 메서드. 프로젝트 CalendarCollection에서 캘린더를 제거합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

프로젝트 CalendarCollection에서 캘린더를 제거합니다.

```csharp
public bool Remove(Calendar item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | Calendar | 제거할 캘린더. |

### 반환 값

제거되면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 캘린더를 제거할 수 없을 때 발생합니다. |

## 예제

컬렉션에서 캘린더를 교체하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// 새 캘린더 추가
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


