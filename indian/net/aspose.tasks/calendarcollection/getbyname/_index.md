---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। निर्दिष्ट नाम के साथ एक कैलेंडर लौटाता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

निर्दिष्ट नाम वाला कैलेंडर लौटाता है।

```csharp
public Calendar GetByName(string name)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | कैलेंडर का नाम। |

### रिटर्न वैल्यू

यदि मिला तो निर्दिष्ट नाम वाले कैलेंडर को लौटाता है, अन्यथा null लौटाता है।

## उदाहरण

दिखाता है कि नाम या आईडी द्वारा कैलेंडर कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


