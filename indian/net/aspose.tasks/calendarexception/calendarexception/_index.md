---
title: "CalendarException.CalendarException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CalendarException कंस्ट्रक्टर। CalendarException क्लास का नया इंस्टेंस प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/calendarexception/calendarexception/
---
## CalendarException constructor

एक नया इंस्टेंस प्रारंभ करता है [`CalendarException`](../) क्लास का।

```csharp
public CalendarException()
```

## उदाहरण

कैलेंडर अपवादों को जोड़ने/हटाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_test.mpp");

// एक कैलेंडर बनाएं
var calendar = project.Calendars.Add("Calendar1");

// छुट्टी के लिए सप्ताह के दिनों का अपवाद बनाएं
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// जाँचें कि तिथि अपवादात्मक है
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// एक अपवाद हटाएँ
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// एक अपवाद जोड़ें
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// अपवादों को प्रिंट करें
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### संबंधित देखें

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


