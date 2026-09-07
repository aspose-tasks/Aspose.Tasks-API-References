---
title: "क्लास CalendarCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalendarCollection क्लास। Calendar ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 240
url: /hi/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

[`Calendar`](../calendar/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class CalendarCollection : IList<Calendar>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | `CalendarCollection` ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | इस CalendarCollection ऑब्जेक्ट में एक नया बेस कैलेंडर जोड़ता है और जोड़ा गया कैलेंडर लौटाता है। |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | निर्दिष्ट बेस कैलेंडर के साथ एक नया कैलेंडर इस CalendarCollection ऑब्जेक्ट में जोड़ता है और जोड़ा गया कैलेंडर लौटाता है। |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | निर्दिष्ट नाम वाला कैलेंडर लौटाता है। |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | निर्दिष्ट UID वाला कैलेंडर लौटाता है। |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | प्रोजेक्ट CalendarCollection से कैलेंडर हटाता है। |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | CalendarCollection ऑब्जेक्ट को [`Calendar`](../calendar/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


