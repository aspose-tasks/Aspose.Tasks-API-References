---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। एक संसाधन का कैलेंडर"
type: docs
weight: 190
url: /hi/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

संसाधन का कैलेंडर।

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## उदाहरण

दिखाता है कि कैसे प्राप्त/सेट करें एक संसाधन कैलेंडर।

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// मानक कैलेंडर जोड़ें और संसाधन को असाइन करें
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// सभी संसाधनों के लिए बेस कैलेंडर नाम प्रदर्शित करें
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


