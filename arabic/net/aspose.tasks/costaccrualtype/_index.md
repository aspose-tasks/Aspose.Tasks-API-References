---
title: "تعداد CostAccrualType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.CostAccrualType. يحدد نوع تكلفة الاستحقاق"
type: docs
weight: 350
url: /ar/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

يحدد نوع تكلفة الاستحقاق.

```csharp
public enum CostAccrualType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن القيمة غير معرفة تعني أن الحقل لم يُعرّف في ملف المشروع الأصلي. |
| Start | `0` | يشير إلى نوع استحقاق التكلفة عند البدء. |
| Prorated | `1` | يشير إلى نوع استحقاق التكلفة بالتقسيط. |
| End | `2` | يشير إلى نوع استحقاق التكلفة عند الانتهاء. |
| Invalid | `3` | يشير إلى نوع استحقاق تكلفة غير صالح. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يعرض كيف ومتى يتم فرض تكاليف الموارد العادية والوقت الإضافي، أو استحقاقها (طريقة الاستحقاق: تحدد متى تُتحمل تكلفة المورد ومتى تُفرض التكاليف الفعلية على المشروع. يمكنك تحمل التكاليف عند البدء [Start] أو الانتهاء [End] من المهمة أو تقسيطها [Prorated] أثناء المهمة.)، لتكلفة المهمة (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// تعيين نوع استحقاق التكلفة
// إذا اخترت خيار الانتهاء، لا يتم استحقاق التكاليف حتى يصبح العمل المتبقي صفرًا.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


