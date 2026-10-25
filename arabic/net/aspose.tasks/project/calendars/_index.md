---
title: "Project.Calendars"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على كائن CalendarCollection لهذا المثال من Project"
type: docs
weight: 130
url: /ar/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

يحصل على كائن [`CalendarCollection`](../../calendarcollection/) لهذا المثال من Project.

```csharp
public CalendarCollection Calendars { get; }
```

## الأمثلة

يعرض كيفية قراءة تقاويم المشروع.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // إظهار ما إذا كان لديه تقويم أساسي
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // احصل على الوقت بالساعات لكل يوم عمل
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### انظر أيضًا

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


