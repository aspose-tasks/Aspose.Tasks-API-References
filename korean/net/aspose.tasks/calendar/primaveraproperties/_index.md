---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. Primavera 형식에서 읽은 캘린더에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Primavera 형식에서 읽은 캘린더에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## 예제

Primavera 파일에서 프로젝트를 읽고 캘린더의 Primavera 전용 속성을 검사하는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### 또 보기

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


