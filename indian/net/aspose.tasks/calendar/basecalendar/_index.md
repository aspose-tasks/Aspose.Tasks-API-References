---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। उस बेस कैलेंडर को प्राप्त या सेट करता है जिस पर यह कैलेंडर निर्भर करता है। केवल तब लागू जब कैलेंडर बेस कैलेंडर न हो।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

इस कैलेंडर पर निर्भर आधार कैलेंडर को प्राप्त करता है या सेट करता है। केवल तब लागू होता है जब कैलेंडर आधार कैलेंडर नहीं है।

```csharp
public Calendar BaseCalendar { get; set; }
```

## उदाहरण

संसाधन के कैलेंडर के बेस कैलेंडर के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// मानक कैलेंडर जोड़ें और संसाधन को असाइन करें
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// सभी संसाधनों के लिए बेस कैलेंडर नाम प्रदर्शित करें
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


