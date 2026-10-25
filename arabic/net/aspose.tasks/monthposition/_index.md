---
title: "Enum MonthPosition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.MonthPosition enum. يحدد موضع عنصر الشهر داخل الشهر"
type: docs
weight: 1070
url: /ar/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

يحدد موضع عنصر الشهر داخل الشهر.

```csharp
public enum MonthPosition
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى موضع شهر غير معرف. |
| First | `0` | يشير إلى موضع شهر أول. |
| Second | `1` | يشير إلى موضع شهر ثاني. |
| Third | `2` | يشير إلى موضع شهر ثالث. |
| Fourth | `3` | يشير إلى موضع الشهر الرابع. |
| Last | `4` | يشير إلى موضع الشهر الأخير. |

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


