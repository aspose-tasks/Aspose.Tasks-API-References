---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. 이 캘린더가 의존하는 기본 캘린더를 가져오거나 설정합니다. 캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

이 캘린더가 의존하는 기본 캘린더를 가져오거나 설정합니다. 캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다.

```csharp
public Calendar BaseCalendar { get; set; }
```

## 예제

리소스 캘린더의 기본 캘린더를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// 표준 캘린더를 추가하고 리소스에 할당합니다.
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// 모든 리소스에 대한 기본 캘린더 이름 표시
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


