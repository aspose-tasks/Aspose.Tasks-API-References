---
title: "Prj.Calendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 캘린더"
type: docs
weight: 90
url: /ko/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

프로젝트 달력.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## 예제

Shows how to read/write Prj.Calendar property.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

project.Set(Prj.Calendar, calendar);

Console.WriteLine("Calendar: " + project.Get(Prj.Calendar).Name);
foreach (var weekDay in calendar.WeekDays)
{
    Console.WriteLine(weekDay.FromDate);
    Console.WriteLine(weekDay.ToDate);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


