---
title: "Aspose::Tasks::Calendar क्लास"
linktitle: "कैलेंडर"
articleTitle: "कैलेंडर"
second_title: "Aspose.Tasks C++ के लिए"
description: "परियोजना में उपयोग किए जाने वाले कैलेंडर का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

परियोजना में उपयोग किए जाने वाले कैलेंडर का प्रतिनिधित्व करता है।

शुरुआत से सरल कैलेंडर कैसे बनाएं।

```cpp
[C#]
// खाली कैलेंडर बनाएं
Calendar calendar = new Calendar("New calendar");
// डिफ़ॉल्ट कार्य दिवस जोड़ता है (9:00 से 17:00 तक 8 कार्य घंटे)
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
// सप्ताहांत जोड़ता है
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```cpp
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

कैलेंडर का उपयोग मानक कार्य और गैर-कार्य समय को परिभाषित करने के लिए किया जाता है। परियोजनाओं के पास एक बेस कैलेंडर होना आवश्यक है। कार्य और संसाधनों के पास अपने स्वयं के गैर-बेस कैलेंडर हो सकते हैं जो एक बेस कैलेंडर पर आधारित होते हैं।

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Delete](./delete/) | परियोजना से कैलेंडर हटाता है। |
| [Equals](./equals/) | वापस देता है एक मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [get_BaseCalendar](./get_basecalendar/) | इस कैलेंडर पर निर्भर बेस कैलेंडर प्राप्त करता है। केवल तब लागू जब कैलेंडर बेस कैलेंडर न हो। |
| [get_Exceptions](./get_exceptions/) | CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी अपवादों का संग्रह। |
| [get_Guid](./get_guid/) | कैलेंडर का Guid प्राप्त करता है। |
| [get_IsBaseCalendar](./get_isbasecalendar/) | एक मान प्राप्त करता है जो दर्शाता है कि कैलेंडर बेस कैलेंडर है या नहीं। |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | एक मान प्राप्त करता है जो दर्शाता है कि कैलेंडर बेसलाइन कैलेंडर है या नहीं। |
| [get_Name](./get_name/) | कैलेंडर का नाम प्राप्त करता है। |
| [get_Uid](./get_uid/) | कैलेंडर की अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [get_WeekDays](./get_weekdays/) | इस कैलेंडर के लिए WeekDaysCollection प्राप्त करता है। कैलेंडर को परिभाषित करने वाले weekdays का संग्रह। |
| [get_WorkWeeks](./get_workweeks/) | WorkWeekCollections ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी कार्य सप्ताहों का संग्रह। |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करता है। |
| [GetHashCode](./gethashcode/) | क्लास की इंस्टेंस के लिए हैश कोड लौटाता है। |
| [GetIntersectionCalendar](./getintersectioncalendar/) | ICalendar इंस्टेंस प्राप्त करता है जिसका उपयोग दो कैलेंडरों के कार्य शेड्यूल के प्रतिच्छेदन पर गणनाएँ करने के लिए किया जा सकता है। |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है। |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | निर्दिष्ट तिथि से पिछले कार्य दिवस के अंत की गणना करता है। |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | कार्य की प्रारंभ तिथि, विभाजित भाग और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है। |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | निर्दिष्ट तिथियों के बीच कार्य घंटे की मात्रा लौटाता है। |
| [GetWorkingTimes](./getworkingtimes/) | निर्दिष्ट तिथि के लिए कार्य समय की WorkingTimeCollection लौटाता है। |
| [GetWorkStart](./getworkstart/) | निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है। |
| [IsDayWorking](./isdayworking/) | निर्धारित करता है कि निर्दिष्ट दिन कैलेंडर के अनुसार कार्य दिवस है या नहीं। |
| [IsEmpty](./isempty/) | वापस देता है कि कैलेंडर में कार्य घंटे परिभाषित नहीं हैं। |
| [Make24HourCalendar](./make24hourcalendar/) | दिए गए कैलेंडर को 24Hour कैलेंडर बनाता है। 24Hours कैलेंडर वह कैलेंडर है जिसमें सप्ताह के हर दिन निरंतर कार्य घंटे होते हैं। |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | दिए गए कैलेंडर को Night Shift कैलेंडर बनाता है। |
| [MakeStandardCalendar](./makestandardcalendar/) | डिफ़ॉल्ट मानक कैलेंडर बनाता है। |
| [set_BaseCalendar](./set_basecalendar/) | इस कैलेंडर पर निर्भर बेस कैलेंडर सेट करता है। केवल तब लागू जब कैलेंडर बेस कैलेंडर न हो। |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | एक मान सेट करता है जो दर्शाता है कि कैलेंडर बेसलाइन कैलेंडर है या नहीं। |
| [set_Name](./set_name/) | कैलेंडर का नाम सेट करता है। |
| [set_Uid](./set_uid/) | कैलेंडर की अद्वितीय पहचानकर्ता सेट करता है। |

