---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। इस CalendarCollection ऑब्जेक्ट में एक नया बेस कैलेंडर जोड़ता है और जोड़ा गया कैलेंडर लौटाता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

इस CalendarCollection ऑब्जेक्ट में एक नया बेस कैलेंडर जोड़ता है और जोड़ा गया कैलेंडर लौटाता है।

```csharp
public Calendar Add(string name)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | कैलेंडर नाम। |

### रिटर्न वैल्यू

जोड़ा गया [`Calendar`](../../calendar/) ऑब्जेक्ट।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब कैलेंडर नाम null हो तो थ्रो किया जाता है। |

## उदाहरण

दिखाता है कि मानक कैलेंडर कैसे बनाएं।

```csharp
var project = new Project();

// एक कैलेंडर परिभाषित करें और उसे मानक बनाएं
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

निर्दिष्ट बेस कैलेंडर के साथ एक नया कैलेंडर इस CalendarCollection ऑब्जेक्ट में जोड़ता है और जोड़ा गया कैलेंडर लौटाता है।

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | निर्दिष्ट नाम। |
| baseCalendar | कैलेंडर | निर्दिष्ट बेस कैलेंडर। |

### रिटर्न वैल्यू

जोड़ा गया [`Calendar`](../../calendar/) ऑब्जेक्ट।

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


