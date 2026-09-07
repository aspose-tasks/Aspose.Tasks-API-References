---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है"
type: docs
weight: 180
url: /hi/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है।

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| तारीख | DateTime | वह तिथि जिसके लिए अगले कार्य दिवस की शुरुआत प्राप्त करनी है। |

### रिटर्न वैल्यू

अगले कार्य दिवस की शुरुआत का DateTime।

## उदाहरण

कैलेंडर का उपयोग करके अगले कार्य दिवस की शुरुआत प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// अगले कार्य दिवस की शुरुआत प्राप्त करें (सप्ताहांत को छोड़ दिया जाता है)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 अप्रैल 2020 9:00 AM प्रिंट किया जाएगा
Console.WriteLine(nextWorkingDayStart);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


