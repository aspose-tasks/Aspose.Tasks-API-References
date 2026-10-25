---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar विधि। दिए गए कैलेंडर को नाइट शिफ्ट कैलेंडर बनाती है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

दिए गए कैलेंडर को नाइट शिफ्ट कैलेंडर बनाता है।

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कैलेंडर | कैलेंडर | नाइट शिफ्ट कैलेंडर बनाने के लिए कैलेंडर। |

### रिटर्न वैल्यू

नाइट शिफ्ट कैलेंडर।

## उदाहरण

दिखाता है कि नाइट शिफ्ट कैलेंडर कैसे बनाएं।

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// कार्य घंटे दिखाएँ
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

दिखाता है कि कैलेंडर को नाइट शिफ्ट कैलेंडर में कैसे बदलें।

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// कार्य घंटे दिखाएँ
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


