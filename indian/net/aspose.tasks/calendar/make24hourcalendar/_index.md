---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। दिए गए कैलेंडर को 24 घंटे वाला कैलेंडर बनाता है। 24 घंटे वाला कैलेंडर वह कैलेंडर है जिसमें सप्ताह के हर दिन राउंड-द-कलॉक कार्य घंटे के साथ काम करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

दिए गए कैलेंडर को 24Hour Calendar बनाता है। 24Hours Calendar वह कैलेंडर है जिसमें सप्ताह के हर दिन राउंड-द- clock कार्य घंटे के साथ काम करता है।

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कैलेंडर | कैलेंडर | Calendar से 24 घंटे का कैलेंडर बनाने के लिए। |

### रिटर्न वैल्यू

24Hour कैलेंडर।

## उदाहरण

दिखाता है कि 24 घंटे का कैलेंडर कैसे बनाएं।

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 घंटे प्रिंट किए जाएंगे
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

दिखाता है कि नए कैलेंडर को 24 घंटे के कैलेंडर में कैसे बदलें।

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 घंटे प्रिंट किए जाएंगे
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


