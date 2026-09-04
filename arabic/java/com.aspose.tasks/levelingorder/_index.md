---
title: "LevelingOrder"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يعرف القيم الممكنة لترتيب التسوية."
type: docs
weight: 143
url: /ar/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

يعرف القيم الممكنة لترتيب التسوية.
## الحقول

| حقل | الوصف |
| --- | --- |
| [IdOnly](#IdOnly) | يتم تأخير المهام بترتيب تصاعدي للمعرف. |
| [PriorityThenStandard](#PriorityThenStandard) | يُؤخذ الأولوية في الاعتبار أولاً، ثم نفس الخصائص كما في الوضع القياسي. |
| [Standard](#Standard) | يتم أخذ الخصائص التالية في الاعتبار: علاقات السلف، الفائض الكلي (المهمة التي لديها فائض كلي أعلى تُؤخر أولاً)، تاريخ البدء، الأولوية. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


يتم تأخير المهام بترتيب تصاعدي للمعرف.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


يُؤخذ الأولوية في الاعتبار أولاً، ثم نفس الخصائص كما في الوضع القياسي.

### Standard {#Standard}
```
public static final int Standard
```


يتم أخذ الخصائص التالية في الاعتبار: علاقات السلف، الفائض الكلي (المهمة التي لديها فائض كلي أعلى تُؤخر أولاً)، تاريخ البدء، الأولوية. هذه هي القيمة الافتراضية.

