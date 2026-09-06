---
title: "التعداد CalendarExceptionType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.CalendarExceptionType. يحدد نوع استثناء التقويم"
type: docs
weight: 270
url: /ar/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

يحدد نوع استثناء التقويم.

```csharp
public enum CalendarExceptionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Daily | `0` | يشير إلى نوع الاستثناء اليومي. |
| YearlyByDay | `1` | يشير إلى نوع الاستثناء السنوي حسب يوم الشهر. |
| YearlyByPosition | `2` | يشير إلى نوع الاستثناء السنوي حسب الموقع. |
| MonthlyByDay | `3` | يشير إلى نوع الاستثناء الشهري حسب يوم الشهر. |
| MonthlyByPosition | `4` | يشير إلى نوع الاستثناء الشهري حسب الموقع. |
| Weekly | `5` | يشير إلى نوع الاستثناء الأسبوعي. |
| ByDayCount | `6` | يشير إلى نوع الاستثناء حسب عدد الأيام. |
| ByWeekDayCount | `7` | يشير إلى نوع الاستثناء حسب عدد أيام الأسبوع. |
| NoExceptionType | `8` | يشير إلى عدم وجود نوع استثناء. |

## الأمثلة

يوضح كيفية تعريف استثناء تقويم حسب التكرارات.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// حدد الاستثناء وحدد التكرارات
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// إضافة استثناء إلى التقويم
calendar.Exceptions.Add(exception);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


