---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException property. प्राप्त करता है या सेट करता है उन घटनाओं की संख्या जिसके लिए कैलेंडर अपवाद मान्य है"
type: docs
weight: 110
url: /hi/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

कैलेंडर अपवाद के मान्य होने की घटनाओं की संख्या प्राप्त करता या सेट करता है।

```csharp
public int Occurrences { get; set; }
```

## उदाहरण

दिखाता है कि घटनाओं द्वारा कैलेंडर अपवाद कैसे परिभाषित किया जाए।

```csharp
var project = new Project();

// कैलेंडर परिभाषित करें
var calendar = project.Calendars.Add("Calendar1");

// अपवाद को परिभाषित करें और घटनाओं को निर्दिष्ट करें
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// कैलेंडर में अपवाद जोड़ें
calendar.Exceptions.Add(exception);
```

### संबंधित देखें

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


