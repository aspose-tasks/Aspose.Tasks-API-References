---
title: "WorkUnit.WorkingHours"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkUnit प्रॉपर्टी। प्राप्त करता है या सेट करता है कार्य घंटे की अवधि"
type: docs
weight: 40
url: /hi/net/aspose.tasks/workunit/workinghours/
---
## WorkUnit.WorkingHours property

कार्य घंटों की अवधि को प्राप्त करता है या सेट करता है।

```csharp
public TimeSpan WorkingHours { get; set; }
```

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


