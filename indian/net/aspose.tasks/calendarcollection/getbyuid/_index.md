---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarCollection मेथड। निर्दिष्ट UID वाले कैलेंडर को लौटाता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

निर्दिष्ट UID वाला कैलेंडर लौटाता है।

```csharp
public Calendar GetByUid(int uid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | Int32 | कैलेंडर का UID। |

### रिटर्न वैल्यू

निर्दिष्ट UID वाला कैलेंडर।

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


