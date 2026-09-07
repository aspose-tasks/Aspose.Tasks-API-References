---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त करता है कि कैलेंडर बेस कैलेंडर है या नहीं"
type: docs
weight: 70
url: /hi/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

यह दर्शाने वाला मान प्राप्त करता है कि कैलेंडर आधार कैलेंडर है या नहीं।

```csharp
public bool IsBaseCalendar { get; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट कैलेंडर और उनकी प्रॉपर्टीज़ कैसे पढ़ें।

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

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


