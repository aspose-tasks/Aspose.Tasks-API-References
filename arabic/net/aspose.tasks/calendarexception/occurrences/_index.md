---
title: "CalendarException.Occurrences"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. يحصل أو يحدد عدد التكرارات التي يكون فيها استثناء التقويم صالحًا"
type: docs
weight: 110
url: /ar/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

يحصل أو يضبط عدد مرات التكرار التي يكون فيها استثناء التقويم صالحًا.

```csharp
public int Occurrences { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


