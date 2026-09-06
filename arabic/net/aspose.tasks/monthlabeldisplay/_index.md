---
title: "تعداد MonthLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.MonthLabelDisplay enum. يحدد كيفية عرض تسمية الشهر"
type: docs
weight: 1060
url: /ar/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

يحدد كيفية عرض تسمية الشهر.

```csharp
public enum MonthLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Mo | `0` | يضبط قائمة الأشهر في MS Project كـ mo. |
| Mon | `1` | يضبط قائمة الأشهر في MS Project كـ mon. |
| Month | `2` | يضبط قائمة الأشهر في MS Project كـ month. |

## الأمثلة

يوضح كيفية ضبط تسمية الشهر في خيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ضبط كيفية عرض تسمية الشهر
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


