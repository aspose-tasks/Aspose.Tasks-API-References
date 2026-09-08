---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 캘린더"
type: docs
weight: 190
url: /ko/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

리소스의 캘린더.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## 예제

리소스 캘린더를 가져오고/설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// 표준 캘린더를 추가하고 리소스에 할당합니다.
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// 모든 리소스에 대한 기본 캘린더 이름 표시
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


