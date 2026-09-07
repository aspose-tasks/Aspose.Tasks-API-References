---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्दिष्ट तिथि से पिछले कार्य दिवस के अंत की गणना करता है।"
type: docs
weight: 190
url: /hi/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

निर्दिष्ट तिथि से पिछले कार्य दिवस के अंत की गणना करता है।

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| तारीख | DateTime | पिछले कार्य दिवस के अंत की गणना करने की तिथि। |

### रिटर्न वैल्यू

पिछले कार्य दिवस का अंत।

## उदाहरण

दिखाता है कि कैलेंडर का उपयोग करके पिछले कार्य दिवस के अंत को कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// पिछले कार्य दिवस का अंत प्राप्त करें
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 अप्रैल 2020 18:00 PM प्रिंट किया जाएगा
Console.WriteLine(previousWorkingDayEnd);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


