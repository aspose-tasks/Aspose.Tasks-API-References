---
title: "Enum DayLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.DayLabelDisplay enum. يحدد كيف يتم عرض تسمية اليوم"
type: docs
weight: 440
url: /ar/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

يحدد كيفية عرض تسمية اليوم.

```csharp
public enum DayLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| D | `0` | يضبط قائمة الأيام في MS Project كـ d. |
| Dy | `1` | يضبط قائمة الأيام في MS Project كـ dy. |
| Day | `2` | يضبط قائمة الأيام في MS Project كـ day. |

## الأمثلة

يعرض كيفية ضبط تسمية اليوم لخيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// عيّن طريقة عرض تسمية اليوم
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


