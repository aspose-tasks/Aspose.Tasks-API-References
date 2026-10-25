---
title: "Prj.Calendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट कैलेंडर"
type: docs
weight: 90
url: /hi/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

परियोजना कैलेंडर।

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## उदाहरण

दिखाता है कि Prj.Calendar प्रॉपर्टी को कैसे पढ़ें/लिखें।

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

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


