---
title: "Enum WeekLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.WeekLabelDisplay enum. يحدد كيف يتم عرض تسمية الأسبوع"
type: docs
weight: 3560
url: /ar/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

يحدد كيفية عرض تسمية الأسبوع.

```csharp
public enum WeekLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| W | `0` | "w" التسمية. |
| Wk | `1` | "wk" التسمية. |
| Week | `2` | "week" التسمية. |

## الأمثلة

يعرض كيفية ضبط تسمية الأسبوع لخيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// عيّن طريقة عرض تسمية الأسبوع
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


