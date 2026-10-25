---
title: "UndefinedConstraintHandlingBehavior"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد السلوك المستخدم للتعامل مع المهام ذات القيود غير المعرفة."
type: docs
weight: 329
url: /ar/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

يحدد السلوك المستخدم للتعامل مع المهام ذات القيود غير المعرفة.
## الحقول

| حقل | الوصف |
| --- | --- |
| [None](#None) | السلوك الافتراضي لتحميل من تنسيق XER. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | يتم إضافة قيود من النوع 'ConstraintType.StartNoEarlierThan' وتاريخ = Start للمهام ذات القيد 'Undefined'. |
### None {#None}
```
public static final int None
```


السلوك الافتراضي لتحميل من تنسيق XER. لا يتم اتخاذ أي إجراء. يتم تعيين نوع قيد المهمة إلى 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


يتم إضافة قيود من النوع 'ConstraintType.StartNoEarlierThan' وتاريخ = Start للمهام ذات القيد 'Undefined'.

