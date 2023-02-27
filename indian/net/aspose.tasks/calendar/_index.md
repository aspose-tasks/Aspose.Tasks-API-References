---
title: Calendar
second_title: Aspose.Tasks for .NET API Reference
description: कस प्रजेक्ट में उपयग कए गए कैलेंडर क प्रतनधत्व करत है
type: docs
weight: 230
url: /hi/net/aspose.tasks/calendar/
---
## Calendar class

किसी प्रोजेक्ट में उपयोग किए गए कैलेंडर का प्रतिनिधित्व करता है।

```csharp
public class Calendar
```

## गुण

| नाम | विवरण |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | उस आधार कैलेंडर को प्राप्त या सेट करता है जिस पर यह कैलेंडर निर्भर करता है। केवल तभी लागू होता है जब कैलेंडर आधार कैलेंडर नहीं है। |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़े अपवादों का संग्रह। |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | यह इंगित करने वाला मान प्राप्त करता है कि क्या कैलेंडर एक आधार कैलेंडर है. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि कैलेंडर एक आधारभूत कैलेंडर है। |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | कैलेंडर का नाम प्राप्त या सेट करता है। |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | कैलेंडर का विशिष्ट पहचानकर्ता प्राप्त या सेट करता है। |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | इस कैलेंडर के लिए सप्ताह के दिनों का संग्रह प्राप्त करता है। सप्ताह के दिनों का संग्रह जो कैलेंडर को परिभाषित करता है। |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections ऑब्जेक्ट प्राप्त करता है। कैलेंडर से संबद्ध कार्य सप्ताहों का संग्रह। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | किसी दिए गए कैलेंडर को 24 घंटे का कैलेंडर बनाता है। 24 घंटे का कैलेंडर एक ऐसा कैलेंडर है जिसमें सप्ताह का हर दिन चौबीसों घंटे काम कर रहा है। |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | किसी दिए गए कैलेंडर को नाइट शिफ्ट कैलेंडर के रूप में बनाता है। |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | डिफ़ॉल्ट मानक कैलेंडर बनाता है। |
| [Delete](../../aspose.tasks/calendar/delete/)() | प्रोजेक्ट से कैलेंडर निकालता है। |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | उस तिथि की गणना करता है जब कार्य समय की निर्दिष्ट राशि कैलेंडर के अनुसार बीत जाएगी। |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | उस तिथि की गणना करता है जब कार्य समय की निर्दिष्ट राशि कैलेंडर के अनुसार बीत जाएगी। |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | वर्ग के उदाहरण के लिए हैश कोड लौटाता है। |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | अगले कार्य दिवस की शुरुआत की तारीख से गणना करता है। |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | निर्दिष्ट तिथि से पिछली कार्य तिथि समाप्ति की गणना करता है। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | रिटर्न स्टार्टडेट निर्दिष्ट फिनिशडेट और अवधि के आधार पर। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | रिटर्न स्टार्टडेट निर्दिष्ट फिनिशडेट और अवधि के आधार पर। |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | इसकी प्रारंभ तिथि, विभाजित भागों और अवधि से कार्य समाप्ति तिथि और समय की गणना करता है। |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | तारीख को काम के घंटे लौटाता है। |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | निर्दिष्ट तिथियों के लिए काम के घंटे लौटाएं। |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | रिटर्न[`WorkingTimeCollection`](../workingtimecollection/) निर्दिष्ट तिथि के लिए कार्य समय की। |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | निर्धारित करता है कि दिन कार्य दिवस है या नहीं। |

### टिप्पणियों

कैलेंडर का उपयोग मानक कार्य और गैर-कार्य समय को परिभाषित करने के लिए किया जाता है। परियोजनाओं में एक आधार कैलेंडर होना चाहिए। कार्यों और संसाधनों के पास उनके स्वयं के गैर-आधार कैलेंडर हो सकते हैं जो आधार कैलेंडर पर आधारित होते हैं।

### उदाहरण

स्क्रैच से सरल कैलेंडर कैसे बनाएं।

```csharp
[C#]
// खाली कैलेंडर बनाएं
Calendar calendar = new Calendar("New calendar");
// डिफ़ॉल्ट कार्य दिवस जोड़ता है (8 कार्य घंटे 9:00 से 17:00 तक)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// नया नया कार्य दिवस बनाएं
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// कार्य समय निर्धारित करता है। डेटटाइम का केवल समय भाग महत्वपूर्ण है
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// सप्ताहांत जोड़ता है
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' खाली कैलेंडर बनाएँ
Dim calendar As Calendar =  New Calendar("New calendar")
' डिफ़ॉल्ट कार्य दिवस जोड़ता है (8 कार्य घंटे 9:00 से 17:00 तक)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' नया नया कार्य दिवस बनाएँ
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' कार्य समय निर्धारित करता है। डेटटाइम का केवल समय भाग महत्वपूर्ण है
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' सप्ताहांत जोड़ता है
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### यह सभी देखें

* नाम स्थान [Aspose.Tasks](../../aspose.tasks/)
* सभा [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
