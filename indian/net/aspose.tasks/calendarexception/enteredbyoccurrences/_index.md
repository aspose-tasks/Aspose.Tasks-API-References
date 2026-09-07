---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि आवृत्ति की सीमा घटनाओं की संख्या दर्ज करके निर्धारित की गई है या नहीं। False यह निर्दिष्ट करता है कि आवृत्ति की सीमा समाप्ति तिथि दर्ज करके निर्धारित की गई है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि पुनरावृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित है या नहीं। False यह निर्दिष्ट करता है कि पुनरावृत्ति की सीमा समाप्ति तिथि दर्ज करके परिभाषित है।

```csharp
public bool EnteredByOccurrences { get; set; }
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


