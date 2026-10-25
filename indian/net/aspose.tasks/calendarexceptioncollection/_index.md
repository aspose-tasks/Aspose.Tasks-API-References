---
title: "क्लास CalendarExceptionCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalendarExceptionCollection क्लास। CalendarException ऑब्जेक्ट्स का संग्रह दर्शाती है"
type: docs
weight: 260
url: /hi/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

[`CalendarException`](../calendarexception/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | `CalendarExceptionCollection` ऑब्जेक्ट में सम्मिलित ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | इस ऑब्जेक्ट के लिए पैरेंट कैलेंडर प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | इस संग्रह ऑब्जेक्ट में CalendarException इंस्टेंस जोड़ता है। |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | आंतरिक सूची में अपवादों की रेंज जोड़ता है। |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | `CalendarExceptionCollection` से सभी आइटम हटाता है। |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | इस संग्रह से [`CalendarException`](../calendarexception/) इंस्टेंस हटाता है। |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | CalendarExceptionCollection ऑब्जेक्ट को [`CalendarException`](../calendarexception/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

कैलेंडर अपवाद संग्रह का उपयोग करके कैलेंडर अपवादों को परिभाषित करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// सभी अपवाद हटाएँ
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### संबंधित देखें

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


