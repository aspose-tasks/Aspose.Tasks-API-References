---
title: "تعداد MinuteLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.MinuteLabelDisplay. يحدد كيفية عرض تسمية الدقيقة"
type: docs
weight: 1030
url: /ar/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

يحدد كيفية عرض تسمية الدقيقة.

```csharp
public enum MinuteLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| M | `0` | يعيّن قائمة الدقائق في MS Project كـ m. |
| Min | `1` | يعيّن قائمة الدقائق في MS Project كـ min. |
| Minute | `2` | يعيّن قائمة الدقائق في MS Project كـ minute. |

## الأمثلة

يوضح كيفية تعيين تسمية الدقيقة لخيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// تعيين كيفية عرض تسمية الدقيقة
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


