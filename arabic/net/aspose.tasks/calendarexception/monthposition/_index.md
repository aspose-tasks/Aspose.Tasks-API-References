---
title: "CalendarException.MonthPosition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. يحصل أو يحدد موضع عنصر الشهر داخل الشهر"
type: docs
weight: 90
url: /ar/net/aspose.tasks/calendarexception/monthposition/
---
## CalendarException.MonthPosition property

يحصل أو يضبط موضع عنصر الشهر داخل الشهر.

```csharp
public MonthPosition MonthPosition { get; set; }
```

## الأمثلة

يوضح كيفية تعريف استثناء تقويم حسب يوم الشهر.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// إنشاء تقويم
var calendar = project.Calendars.Add("Calendar1");

// إنشاء استثناء تقويم لكل يوم جمعة
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// تحقق من أن يوم الجمعة استثنائي
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// أضف الاستثناء إلى التقويم
calendar.Exceptions.Add(exception);
```

### انظر أيضًا

* enum [MonthPosition](../../monthposition/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


