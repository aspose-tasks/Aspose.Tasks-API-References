---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। CalendarCollection ऑब्जेक्ट को कैलेंडर ऑब्जेक्ट्स की सूची में परिवर्तित करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

CalendarCollection ऑब्जेक्ट को [`Calendar`](../../calendar/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<Calendar> ToList()
```

### रिटर्न वैल्यू

[`Calendar`](../../calendar/) ऑब्जेक्ट्स की सूची।

## उदाहरण

कैलेंडर कलेक्शन पर इटरेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


