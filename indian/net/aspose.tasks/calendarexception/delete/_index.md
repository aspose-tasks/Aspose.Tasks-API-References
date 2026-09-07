---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException method. पैरेंट कैलेंडर CalendarExceptionCollection ऑब्जेक्ट से Exception इंस्टेंस को हटाता है"
type: docs
weight: 180
url: /hi/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

पैरेंट कैलेंडर CalendarExceptionCollection ऑब्जेक्ट से Exception उदाहरण को हटाता है।

```csharp
public void Delete()
```

## उदाहरण

कैलेंडर अपवाद को हटाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// अपवाद को हटाएँ
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### संबंधित देखें

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


