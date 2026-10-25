---
title: "Project.Calendars"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। इस Project इंस्टेंस का CalendarCollection ऑब्जेक्ट प्राप्त करता है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

इस Project इंस्टेंस का [`CalendarCollection`](../../calendarcollection/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public CalendarCollection Calendars { get; }
```

## उदाहरण

प्रोजेक्ट कैलेंडरों को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // यदि इसमें बेस कैलेंडर है तो दिखाएँ।
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // प्रत्येक कार्य दिवस में घंटे में समय प्राप्त करें।
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### संबंधित देखें

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


