---
title: "Project.Calendars"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 이 Project 인스턴스의 CalendarCollection 객체를 가져옵니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

이 Project 인스턴스의 [`CalendarCollection`](../../calendarcollection/) 객체를 가져옵니다.

```csharp
public CalendarCollection Calendars { get; }
```

## 예제

프로젝트 캘린더를 읽는 방법을 보여줍니다.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


