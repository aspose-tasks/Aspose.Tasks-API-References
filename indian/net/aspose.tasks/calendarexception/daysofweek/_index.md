---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException property. इस ऑब्जेक्ट के लिए DayTypeCollection प्राप्त करता है। वह सप्ताह के दिन जिन पर अपवाद मान्य है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

इस ऑब्जेक्ट के लिए DayTypeCollection प्राप्त करता है। वह सप्ताह के दिन जिन पर अपवाद मान्य है।

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## उदाहरण

सप्ताह के दिन द्वारा कैलेंडर अपवाद को परिभाषित करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_test.mpp");

// एक कैलेंडर बनाएं
var calendar = project.Calendars.Add("Calendar1");

// हर शुक्रवार के लिए कैलेंडर अपवाद बनाएं
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// जाँचें कि शुक्रवार अपवादात्मक है
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// अपवाद को कैलेंडर में जोड़ें
calendar.Exceptions.Add(exception);
```

### संबंधित देखें

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


