---
title: "تعداد UndefinedConstraintHandlingBehavior"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.UndefinedConstraintHandlingBehavior. يحدد السلوك المستخدم للتعامل مع المهام ذات القيود غير المعرفة."
type: docs
weight: 2630
url: /ar/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المحددة.

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | السلوك الافتراضي للتحميل من تنسيق XER. لا يتم اتخاذ أي إجراء. يتم تعيين نوع قيد المهمة إلى 'ConstraintType.Undefined'. |
| SubstituteWithStartNoEarlierThan | `1` | يتم إضافة قيود من النوع 'ConstraintType.StartNoEarlierThan' وتاريخ = Start للمهام ذات القيد 'Undefined'. |

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


