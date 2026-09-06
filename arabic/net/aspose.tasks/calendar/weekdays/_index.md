---
title: "Calendar.WeekDays"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. يحصل على WeekDaysCollection لهذا التقويم. مجموعة أيام الأسبوع التي تحدد التقويم."
type: docs
weight: 120
url: /ar/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

يحصل على WeekDaysCollection لهذا التقويم. مجموعة أيام الأسبوع التي تُعرّف التقويم.

```csharp
public WeekDayCollection WeekDays { get; }
```

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


