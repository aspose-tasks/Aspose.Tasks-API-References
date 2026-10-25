---
title: "التعداد LevelingOrder"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Leveling.LevelingOrder. يحدد القيم الممكنة لترتيب الموازنة"
type: docs
weight: 950
url: /ar/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

يحدد القيم الممكنة لترتيب الموازنة.

```csharp
public enum LevelingOrder
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Standard | `1` | يتم أخذ الخصائص التالية في الاعتبار: علاقات السلف، الفائض الكلي (المهمة التي لديها فائض كلي أعلى تُؤخر أولاً)، تاريخ البدء، الأولوية. هذه هي القيمة الافتراضية. |
| IdOnly | `2` | يتم تأخير المهام بترتيب تصاعدي للمعرف Id. |
| PriorityThenStandard | `3` | تُؤخذ الأولوية في الاعتبار أولاً، ثم نفس الخصائص كما في الوضع Standard. |

### انظر أيضًا

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


