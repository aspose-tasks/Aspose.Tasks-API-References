---
title: "CalendarException.MonthDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarException. يحصل أو يحدد يومًا من الشهر يتم فيه جدولة تكرار الاستثناء"
type: docs
weight: 70
url: /ar/net/aspose.tasks/calendarexception/monthday/
---
## CalendarException.MonthDay property

يحصل أو يضبط يوم الشهر الذي يُجدول فيه تكرار الاستثناء.

```csharp
public int MonthDay { get; set; }
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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


