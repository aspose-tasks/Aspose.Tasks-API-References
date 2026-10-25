---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkUnit कन्स्ट्रक्टर। WorkUnit क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। निर्दिष्ट From और To तिथियों के साथ नया WorkUnit ऑब्जेक्ट बनाता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

[`WorkUnit`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। निर्दिष्ट From और To तिथियों के साथ नया WorkUnit ऑब्जेक्ट बनाता है।

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| से | DateTime | कार्य घंटे की प्रारंभ तिथि। |
| से | DateTime | कार्य घंटे की समाप्ति तिथि। |

## उदाहरण

वर्क यूनिट जानकारी के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// विशिष्ट तिथि के लिए कार्य घंटे प्राप्त करें
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### संबंधित देखें

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


