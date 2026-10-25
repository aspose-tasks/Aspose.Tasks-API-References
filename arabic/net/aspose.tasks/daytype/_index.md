---
title: "التعداد DayType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.DayType. يحدد اليوم في الأسبوع"
type: docs
weight: 450
url: /ar/net/aspose.tasks/daytype/
---
## DayType enumeration

يحدد يوم الأسبوع.

```csharp
public enum DayType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Exception | `0` | يشير إلى نوع يوم الاستثناء. |
| Sunday | `1` | يشير إلى نوع يوم الأحد. |
| Monday | `2` | يشير إلى نوع يوم الاثنين. |
| Tuesday | `3` | يشير إلى نوع يوم الثلاثاء. |
| Wednesday | `4` | يشير إلى نوع يوم الأربعاء. |
| Thursday | `5` | يشير إلى نوع يوم الخميس. |
| Friday | `6` | يشير إلى نوع يوم الجمعة. |
| Saturday | `7` | يشير إلى نوع يوم السبت. |

## الأمثلة

يظهر كيفية تعريف تقويم جديد، إضافة أيام الأسبوع إليه وتعريف أوقات العمل للأيام.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير
var weekDay = new WeekDay(DayType.Friday);

// يضبط وقت العمل. الجزء الزمني فقط من DateTime هو المهم
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


