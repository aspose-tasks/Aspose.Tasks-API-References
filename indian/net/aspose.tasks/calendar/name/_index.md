---
title: "Calendar.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। कैलेंडर का नाम प्राप्त या सेट करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

कैलेंडर का नाम प्राप्त करता है या सेट करता है।

```csharp
public string Name { get; set; }
```

## उदाहरण

दिखाता है कि कैलेंडर जानकारी कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// कैलेंडर की जानकारी प्राप्त करें
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


