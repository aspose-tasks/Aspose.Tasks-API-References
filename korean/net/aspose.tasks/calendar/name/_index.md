---
title: "Calendar.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. 캘린더의 이름을 가져오거나 설정합니다"
type: docs
weight: 90
url: /ko/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

캘린더의 이름을 가져오거나 설정합니다.

```csharp
public string Name { get; set; }
```

## 예제

캘린더 정보를 검색하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// 캘린더 정보 가져오기
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


