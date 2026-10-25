---
title: "एनम CalendarExceptionType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalendarExceptionType एनम। कैलेंडर अपवाद प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 270
url: /hi/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

कैलेंडर अपवाद प्रकार को निर्दिष्ट करता है।

```csharp
public enum CalendarExceptionType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Daily | `0` | दैनिक अपवाद प्रकार दर्शाता है। |
| YearlyByDay | `1` | महीने के दिन द्वारा वार्षिक अपवाद प्रकार दर्शाता है। |
| YearlyByPosition | `2` | स्थिति द्वारा वार्षिक अपवाद प्रकार दर्शाता है। |
| MonthlyByDay | `3` | महीने के दिन द्वारा मासिक अपवाद प्रकार दर्शाता है। |
| MonthlyByPosition | `4` | स्थिति द्वारा मासिक अपवाद प्रकार दर्शाता है। |
| Weekly | `5` | साप्ताहिक अपवाद प्रकार को दर्शाता है। |
| ByDayCount | `6` | दिन गिनती द्वारा अपवाद प्रकार को दर्शाता है। |
| ByWeekDayCount | `7` | हफ़्ते के दिन गिनती द्वारा अपवाद प्रकार को दर्शाता है। |
| NoExceptionType | `8` | कोई अपवाद प्रकार नहीं दर्शाता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


