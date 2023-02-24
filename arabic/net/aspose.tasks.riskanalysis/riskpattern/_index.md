---
title: Class RiskPattern
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.RiskAnalysis.RiskPattern فصل. يمثل نمط مخاطر لمهمة مشروع .
type: docs
weight: 1670
url: /ar/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

يمثل نمط مخاطر لمهمة مشروع .

```csharp
public class RiskPattern
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | يقوم بتهيئة مثيل جديد لملف`RiskPattern` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | الحصول على أو تحديد مستوى الثقة الذي يتوافق مع النسبة المئوية للوقت الذي ستكون فيه القيم الفعلية الناتجة ضمن التقديرات المتفائلة والمتشائمة. القيمة الافتراضية هي CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | الحصول على أو تحديد التوزيع الاحتمالي المستخدم في محاكاة مونت كارلو . القيمة الافتراضية هي ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | الحصول على أو تعيين النسبة المئوية لمدة المهمة الأكثر احتمالاً والتي يمكن أن تحدث في أفضل سيناريو مشروع ممكن . القيمة الافتراضية هي 75 ، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة 4 أيام ، فستكون المدة المتفائلة 3 أيام. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | الحصول على أو تعيين النسبة المئوية لمدة المهمة الأكثر احتمالاً والتي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن. القيمة الافتراضية هي 125 ، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة 4 أيام ، فإن المدة المتشائمة ستكون 5 أيام. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | الحصول على مهمة مشروع يطبق عليها نمط المخاطرة هذا. |

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* المجسم [Aspose.Tasks](../../)


