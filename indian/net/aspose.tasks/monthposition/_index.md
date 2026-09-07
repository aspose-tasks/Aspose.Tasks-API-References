---
title: "Enum MonthPosition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MonthPosition enum. महीने के भीतर महीने के आइटम की स्थिति निर्दिष्ट करता है।"
type: docs
weight: 1070
url: /hi/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

माह के भीतर महीने के आइटम की स्थिति को निर्दिष्ट करता है।

```csharp
public enum MonthPosition
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | अपरिभाषित महीने की स्थिति दर्शाता है। |
| First | `0` | पहली स्थिति महीने की स्थिति दर्शाता है। |
| Second | `1` | दूसरी स्थिति महीने की स्थिति दर्शाता है। |
| Third | `2` | तीसरी स्थिति महीने की स्थिति दर्शाता है। |
| Fourth | `3` | चौथे स्थान के महीने की स्थिति को दर्शाता है। |
| Last | `4` | अंतिम स्थान के महीने की स्थिति को दर्शाता है। |

## उदाहरण

महीने के दिन के आधार पर कैलेंडर अपवाद को परिभाषित करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_test.mpp");

// एक कैलेंडर बनाएं
var calendar = project.Calendars.Add("Calendar1");

// हर शुक्रवार के लिए कैलेंडर अपवाद बनाएं
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// जाँचें कि aa शुक्रवार अपवाद है
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// अपवाद को कैलेंडर में जोड़ें
calendar.Exceptions.Add(exception);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


