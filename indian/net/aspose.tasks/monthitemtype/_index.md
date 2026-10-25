---
title: "Enum MonthItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.MonthItemType enum. उस महीने के आइटम को निर्दिष्ट करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है।"
type: docs
weight: 1050
url: /hi/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

उस महीने के आइटम को निर्दिष्ट करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है।

```csharp
public enum MonthItemType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | अपरिभाषित महीने के आइटम प्रकार को दर्शाता है। |
| Day | `0` | दिन महीने के आइटम प्रकार को दर्शाता है। |
| Weekday | `1` | सप्ताह के कार्यदिवस महीने के आइटम प्रकार को दर्शाता है। |
| WeekendDay | `2` | सप्ताहांत दिन महीने के आइटम प्रकार को दर्शाता है। |
| Sunday | `3` | रविवार महीने के आइटम प्रकार को दर्शाता है। |
| Monday | `4` | सोमवार महीने के आइटम प्रकार को दर्शाता है। |
| Tuesday | `5` | मंगलवार महीने के आइटम प्रकार को दर्शाता है। |
| Wednesday | `6` | बुधवार महीने के आइटम प्रकार को दर्शाता है। |
| Thursday | `7` | गुरुवार महीने के आइटम प्रकार को दर्शाता है। |
| Friday | `8` | शुक्रवार महीने के आइटम प्रकार को दर्शाता है। |
| Saturday | `9` | शनिवार महीने के आइटम प्रकार को दर्शाता है। |

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


