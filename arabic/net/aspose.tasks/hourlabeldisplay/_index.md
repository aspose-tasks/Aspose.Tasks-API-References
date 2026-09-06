---
title: "التعداد HourLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.HourLabelDisplay. يحدد كيفية عرض تسمية الساعة"
type: docs
weight: 820
url: /ar/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

يحدد كيفية عرض تسمية الساعة.

```csharp
public enum HourLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| H | `0` | التسمية "h". |
| Hr | `1` | التسمية "hr". |
| Hour | `2` | التسمية "hour(s)". |

## الأمثلة

يعرض كيفية تعيين تسمية الساعة لخيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// تحديد كيفية عرض تسمية الساعة
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


