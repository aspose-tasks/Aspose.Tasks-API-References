---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। इस कलेक्शन के लिए एक एनेमरेटर लौटाता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### रिटर्न वैल्यू

इस संग्रह के लिए एक एनेमरेटर।

## उदाहरण

नए कैलेंडर जोड़ने का तरीका दिखाता है।

```csharp
var project = new Project();

// कलेक्शन के Add ओवरलोड का उपयोग करके प्रोजेक्ट के कैलेंडर कलेक्शन में नए कैलेंडर जोड़े जा सकते हैं।
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


