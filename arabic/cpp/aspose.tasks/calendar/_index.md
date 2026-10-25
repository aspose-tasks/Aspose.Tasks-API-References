---
title: "فئة Aspose::Tasks::Calendar"
linktitle: "تقويم"
articleTitle: "تقويم"
second_title: "Aspose.Tasks لـ C++"
description: "يمثل تقويمًا يُستخدم في مشروع."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

يمثل تقويمًا يُستخدم في مشروع.

كيفية إنشاء تقويم بسيط من الصفر.

```cpp
[C#]
// إنشاء تقويم فارغ
Calendar calendar = new Calendar("New calendar");
// يضيف أيام عمل افتراضية (8 ساعات عمل من 9:00 إلى 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// إنشاء يوم عمل جديد
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// يضبط وقت العمل. الجزء الزمني فقط من DateTime هو المهم
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
// يضيف عطلة نهاية الأسبوع
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

يُستخدم التقويم لتحديد أوقات العمل القياسية وغير العمل. يجب أن يكون للمشروعات تقويم أساسي واحد. يمكن للمهام والموارد أن يكون لها تقويمات غير أساسية خاصة بها تعتمد على التقويم الأساسي.

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Delete](./delete/) | يزيل التقويم من المشروع. |
| [Equals](./equals/) | يرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن محدد. |
| [get_BaseCalendar](./get_basecalendar/) | يحصل على التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا. |
| [get_Exceptions](./get_exceptions/) | يحصل على كائن CalendarExceptionCollection. مجموعة الاستثناءات المرتبطة بالتقويم. |
| [get_Guid](./get_guid/) | يحصل على معرف الـ Guid للتقويم. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا. |
| [get_Name](./get_name/) | يحصل على اسم التقويم. |
| [get_Uid](./get_uid/) | يحصل على المعرف الفريد للتقويم. |
| [get_WeekDays](./get_weekdays/) | يحصل على WeekDaysCollection لهذا التقويم. مجموعة أيام الأسبوع التي تحدد التقويم. |
| [get_WorkWeeks](./get_workweeks/) | يحصل على كائن WorkWeekCollections. مجموعة أسابيع العمل المرتبطة بالتقويم. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | يحسب التاريخ الذي سينقضي فيه مقدار الوقت العمل المحدد وفقًا للتقويم. |
| [GetHashCode](./gethashcode/) | يعيد رمز تجزئة (hash code) لنسخة الفئة. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | يحصل على نسخة ICalendar التي يمكن استخدامها لإجراء حسابات على تقاطع جداول العمل لتقويمين. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | يحسب بداية يوم العمل التالي للتاريخ المحدد. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | يحسب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة، ومدة العمل. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | يعيد مقدار ساعات العمل في التاريخ المحدد. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | يعيد مقدار ساعات العمل بين التواريخ المحددة. |
| [GetWorkingTimes](./getworkingtimes/) | يعيد WorkingTimeCollection لأوقات العمل للتاريخ المحدد. |
| [GetWorkStart](./getworkstart/) | يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين. |
| [IsDayWorking](./isdayworking/) | يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم. |
| [IsEmpty](./isempty/) | يعيد ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة. |
| [Make24HourCalendar](./make24hourcalendar/) | يجعل التقويم المحدد تقويمًا 24 ساعة. تقويم 24 ساعة هو تقويم يعمل فيه كل يوم من الأسبوع على مدار الساعة. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | يجعل التقويم المحدد تقويمًا بنظام الوردية الليلية. |
| [MakeStandardCalendar](./makestandardcalendar/) | ينشئ تقويمًا قياسيًا افتراضيًا. |
| [set_BaseCalendar](./set_basecalendar/) | يضبط التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | يضبط قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا. |
| [set_Name](./set_name/) | يضبط اسم التقويم. |
| [set_Uid](./set_uid/) | يضبط المعرف الفريد للتقويم. |

