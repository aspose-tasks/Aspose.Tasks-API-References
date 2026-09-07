---
title: "क्लास Calendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Calendar क्लास। परियोजना में उपयोग किए जाने वाले कैलेंडर का प्रतिनिधित्व करता है।"
type: docs
weight: 230
url: /hi/net/aspose.tasks/calendar/
---
## Calendar class

प्रोजेक्ट में उपयोग किए जाने वाले कैलेंडर का प्रतिनिधित्व करता है।

```csharp
public class Calendar : ICalendar
```

## गुण

| नाम | विवरण |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | इस कैलेंडर पर निर्भर आधार कैलेंडर को प्राप्त करता है या सेट करता है। केवल तब लागू होता है जब कैलेंडर आधार कैलेंडर नहीं है। |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी अपवादों का संग्रह। |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | कैलेंडर का Guid प्राप्त करता है। |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | यह दर्शाने वाला मान प्राप्त करता है कि कैलेंडर आधार कैलेंडर है या नहीं। |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | कैलेंडर बेसलाइन कैलेंडर है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | कैलेंडर का नाम प्राप्त करता है या सेट करता है। |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Primavera फ़ॉर्मेट से पढ़े गए कैलेंडर के लिए Primavera-विशिष्ट गुणों वाला ऑब्जेक्ट प्राप्त करता है। |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | कैलेंडर की अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है। |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | इस कैलेंडर के लिए WeekDaysCollection प्राप्त करता है। कैलेंडर को परिभाषित करने वाले weekdays का संग्रह। |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी कार्य सप्ताहों का संग्रह। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | दिए गए कैलेंडर को 24Hour Calendar बनाता है। 24Hours Calendar वह कैलेंडर है जिसमें सप्ताह के हर दिन राउंड-द- clock कार्य घंटे के साथ काम करता है। |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | दिए गए कैलेंडर को नाइट शिफ्ट कैलेंडर बनाता है। |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | डिफ़ॉल्ट मानक कैलेंडर बनाता है। |
| [Delete](../../aspose.tasks/calendar/delete/)() | प्रोजेक्ट से कैलेंडर हटाता है। |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है। |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है। |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | क्लास की इंस्टेंस के लिए हैश कोड लौटाता है। |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है। |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | निर्दिष्ट तिथि से पिछले कार्य दिवस के अंत की गणना करता है। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | कार्य की प्रारंभ तिथि, विभाजित भागों और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है। |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | वर्कयूनिट लौटाता है - निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की शुरुआत, समाप्ति और अवधि। |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | निर्दिष्ट तिथियों के बीच कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | निर्दिष्ट तिथि के लिए कार्य समय की [`WorkingTimeCollection`](../workingtimecollection/) लौटाता है। |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है। |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं। |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | वापस देता है कि क्या कैलेंडर में कार्य घंटे परिभाषित नहीं हैं। |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | [`ICalendar`](../icalendar/) इंस्टेंस प्राप्त करता है जिसका उपयोग दो कैलेंडरों के कार्य शेड्यूल के इंटरसेक्शन पर गणनाएँ करने के लिए किया जा सकता है। |

## टिप्पणियाँ

कैलेंडरों का उपयोग मानक कार्य और गैर-कार्य समय निर्धारित करने के लिए किया जाता है। प्रोजेक्ट्स के पास एक बेस कैलेंडर होना चाहिए। कार्य और संसाधनों के पास अपने स्वयं के नॉन-बेस कैलेंडर हो सकते हैं जो एक बेस कैलेंडर पर आधारित होते हैं।

## उदाहरण

शुरुआत से सरल कैलेंडर कैसे बनाएं।

```csharp
[C#]
// खाली कैलेंडर बनाएं
Calendar calendar = new Calendar("New calendar");
// डिफ़ॉल्ट कार्य दिवस जोड़ता है (9:00 से 17:00 तक 8 कार्य घंटे)।
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// नया कार्य दिवस बनाएं
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// कार्य समय सेट करता है। केवल DateTime का समय भाग महत्वपूर्ण है।
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
// वीकेंड जोड़ता है
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

दिखाता है कि नया कैलेंडर कैसे परिभाषित करें, उसमें सप्ताह के दिन जोड़ें और दिनों के लिए कार्य समय निर्धारित करें।

```csharp
var project = new Project();

// कैलेंडर परिभाषित करें
var calendar = project.Calendars.Add("Calendar1");

// सोमवार से गुरुवार तक डिफ़ॉल्ट समय के साथ कार्य दिवस जोड़ें
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// शुक्रवार को छोटा कार्य दिवस सेट करें
var weekDay = new WeekDay(DayType.Friday);

// कार्य समय सेट करता है। केवल DateTime का समय भाग महत्वपूर्ण है।
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// प्रोजेक्ट के साथ काम कर रहे हैं...
```

### संबंधित देखें

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


