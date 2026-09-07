---
title: "क्लास WorkUnit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WorkUnit क्लास। कार्य घंटे दर्शाता है"
type: docs
weight: 3630
url: /hi/net/aspose.tasks/workunit/
---
## WorkUnit class

कार्य घंटे दर्शाता है।

```csharp
public class WorkUnit
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | `WorkUnit` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। निर्दिष्ट From और To तिथियों के साथ नया WorkUnit ऑब्जेक्ट बनाता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | From तिथि को प्राप्त करता है या सेट करता है। |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | To तिथि को प्राप्त करता है या सेट करता है। |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | कार्य घंटों की अवधि को प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


