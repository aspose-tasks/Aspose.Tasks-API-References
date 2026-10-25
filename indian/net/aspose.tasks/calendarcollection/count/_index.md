---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection प्रॉपर्टी। इस CalendarCollection ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

इस [`CalendarCollection`](../) ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है।

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


