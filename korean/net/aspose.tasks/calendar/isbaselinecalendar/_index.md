---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. 캘린더가 기준선 캘린더인지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

캘린더가 기준선 캘린더인지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## 예제

캘린더가 기준선 캘린더인지 여부를 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


