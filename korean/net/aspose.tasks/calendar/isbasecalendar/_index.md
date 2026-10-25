---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. 캘린더가 기본 캘린더인지 여부를 나타내는 값을 가져옵니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

캘린더가 기본 캘린더인지 여부를 나타내는 값을 가져옵니다.

```csharp
public bool IsBaseCalendar { get; }
```

## 예제

프로젝트 캘린더와 해당 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // 기본 캘린더가 있는지 표시합니다.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // 각 작업일의 시간을 시간 단위로 가져옵니다.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


