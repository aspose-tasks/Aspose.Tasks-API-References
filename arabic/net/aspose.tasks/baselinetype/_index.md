---
title: "تعداد BaselineType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.BaselineType. يحدد نوع الخط الأساسي المستخدم لحساب قيم التباين."
type: docs
weight: 130
url: /ar/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

يحدد نوع الخط الأساسي المستخدم لحساب قيم التباين.

```csharp
public enum BaselineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن الحقل لم يتم تعريفه في ملف المشروع الأصلي. |
| Baseline | `0` | يشير إلى نوع الخط الأساسي. |
| Baseline1 | `1` | يشير إلى نوع Baseline1. |
| Baseline2 | `2` | يشير إلى نوع Baseline2. |
| Baseline3 | `3` | يشير إلى نوع Baseline3. |
| Baseline4 | `4` | يشير إلى نوع Baseline4. |
| Baseline5 | `5` | يشير إلى نوع Baseline5. |
| Baseline6 | `6` | يشير إلى نوع Baseline6. |
| Baseline7 | `7` | يشير إلى نوع Baseline7. |
| Baseline8 | `8` | يشير إلى نوع Baseline8. |
| Baseline9 | `9` | يشير إلى نوع Baseline9. |
| Baseline10 | `10` | يشير إلى نوع Baseline10. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يعرض كيفية تعيين الخط الأساسي للمشروع (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// احفظ حقول الخط الأساسي إلى الخط الأساسي المحدد لكامل المشروع.
project.SetBaseline(BaselineType.Baseline);
// العمل مع خطوط الأساس الخاصة بالمشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


