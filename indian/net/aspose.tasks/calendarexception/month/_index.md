---
title: "CalendarException.Month"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException property. प्राप्त करता है या सेट करता है वह महीना जिसके लिए अपवाद पुनरावृत्ति निर्धारित है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/calendarexception/month/
---
## CalendarException.Month property

उस महीने को प्राप्त करता या सेट करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है।

```csharp
public Month Month { get; set; }
```

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

* enum [Month](../../month/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


