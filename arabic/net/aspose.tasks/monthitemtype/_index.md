---
title: "تعداد MonthItemType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.MonthItemType. يحدد عنصر الشهر الذي يُجدول له تكرار استثناء."
type: docs
weight: 1050
url: /ar/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

يحدد عنصر الشهر الذي يتم جدولة تكرار الاستثناء له.

```csharp
public enum MonthItemType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى نوع عنصر شهر غير معرف. |
| Day | `0` | يشير إلى نوع عنصر شهر يوم. |
| Weekday | `1` | يشير إلى نوع عنصر شهر يوم عمل. |
| WeekendDay | `2` | يشير إلى نوع عنصر شهر يوم عطلة نهاية الأسبوع. |
| Sunday | `3` | يشير إلى نوع عنصر شهر الأحد. |
| Monday | `4` | يشير إلى نوع عنصر شهر الاثنين. |
| Tuesday | `5` | يشير إلى نوع عنصر شهر الثلاثاء. |
| Wednesday | `6` | يشير إلى نوع عنصر شهر الأربعاء. |
| Thursday | `7` | يشير إلى نوع عنصر شهر الخميس. |
| Friday | `8` | يشير إلى نوع عنصر شهر الجمعة. |
| Saturday | `9` | يشير إلى نوع عنصر شهر السبت. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


