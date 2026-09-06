---
title: "CalendarException.EnteredByOccurrences"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. تحصل أو تعيين قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد من التكرارات. False يحدد أن نطاق التكرار معرف بإدخال تاريخ الانتهاء"
type: docs
weight: 40
url: /ar/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

يحصل أو يضبط قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد مرات التكرار. القيمة False تعني أن نطاق التكرار معرف بإدخال تاريخ الانتهاء.

```csharp
public bool EnteredByOccurrences { get; set; }
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


