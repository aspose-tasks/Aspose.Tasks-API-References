---
title: "क्लास CalendarException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalendarException क्लास। कैलेंडर में असाधारण समय अवधि को दर्शाती है"
type: docs
weight: 250
url: /hi/net/aspose.tasks/calendarexception/
---
## CalendarException class

कैलेंडर में असाधारण समय अवधियों को दर्शाता है।

```csharp
public sealed class CalendarException
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [CalendarException](calendarexception/)() | `CalendarException` क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | इस ऑब्जेक्ट के लिए DayTypeCollection प्राप्त करता है। वह सप्ताह के दिन जिन पर अपवाद मान्य है। |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि पुनरावृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित है या नहीं। False यह निर्दिष्ट करता है कि पुनरावृत्ति की सीमा समाप्ति तिथि दर्ज करके परिभाषित है। |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | अपवाद समय की शुरुआत प्राप्त करता या सेट करता है। |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | उस महीने को प्राप्त करता या सेट करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है। |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | उस महीने के दिन को प्राप्त करता या सेट करता है जिस पर अपवाद पुनरावृत्ति निर्धारित है। |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | उस महीने के आइटम को प्राप्त करता या सेट करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है। |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | एक महीने के भीतर महीने के आइटम की स्थिति प्राप्त करता या सेट करता है। |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | अपवाद का नाम प्राप्त करता या सेट करता है। |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | कैलेंडर अपवाद के मान्य होने की घटनाओं की संख्या प्राप्त करता या सेट करता है। |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | इस ऑब्जेक्ट के लिए पैरेंट कैलेंडर प्राप्त करता है। |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | अपवाद के लिए पुनरावृत्ति अवधि प्राप्त करता या सेट करता है। |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | अपवाद समय के अंत को प्राप्त करता या सेट करता है। |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | अपवाद प्रकार प्राप्त करता या सेट करता है। |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | WorkingTimeCollection ऑब्जेक्ट प्राप्त करता या सेट करता है। कार्य दिवस पर काम किए गए समय को परिभाषित करने वाले कार्य समयों का संग्रह। कम से कम एक कार्य समय मौजूद होना चाहिए, और अधिकतम पाँच से अधिक नहीं हो सकता। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | यदि निर्दिष्ट DateTime स्ट्रक्ट का उदाहरण अपवाद दिवस है तो true लौटाता है। |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | पैरेंट कैलेंडर CalendarExceptionCollection ऑब्जेक्ट से Exception उदाहरण को हटाता है। |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | उन तिथियों को लौटाता है जिन पर कैलेंडर अपवाद लागू होता है। |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | कैलेंडर अपवाद के लिए कार्य समय लौटाता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


