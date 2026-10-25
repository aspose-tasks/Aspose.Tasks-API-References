---
title: "تعداد YearLabelDisplay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.YearLabelDisplay. يحدد كيفية عرض تسمية السنة"
type: docs
weight: 3680
url: /ar/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

يحدد كيفية عرض تسمية السنة.

```csharp
public enum YearLabelDisplay
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Y | `0` | يضبط قائمة السنوات في MS Project كـ mo. |
| Yr | `1` | يضبط قائمة السنوات في MS Project كـ mon. |
| Year | `2` | يضبط قائمة السنوات في MS Project كشهر. |

## الأمثلة

يعرض كيفية ضبط تسمية السنة في خيارات عرض المشروع (الحالة 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ضبط كيفية عرض تسمية السنة
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


