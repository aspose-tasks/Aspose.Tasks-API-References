---
title: "Calendar.MakeStandardCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। डिफ़ॉल्ट मानक कैलेंडर बनाता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

डिफ़ॉल्ट मानक कैलेंडर बनाता है।

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कैलेंडर | कैलेंडर | मानक कैलेंडर बनाने के लिए Calendar |

### रिटर्न वैल्यू

कैलेंडर जिसमें 5 कार्य दिवस (सोमवार-शुक्रवार) हैं, कार्य समय 8-12 और 13-17।

## उदाहरण

मानक कैलेंडर बनाने का तरीका दिखाता है।

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// कार्य घंटे दिखाएँ
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

अपवाद दिनों के साथ कैलेंडर बनाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// कैलेंडर जानकारी अपडेट करें
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


