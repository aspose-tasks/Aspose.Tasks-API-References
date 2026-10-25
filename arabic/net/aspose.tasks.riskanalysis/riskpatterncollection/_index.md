---
title: "الفئة RiskPatternCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection class. تمثل مجموعة تحتوي على مثيلات فئة RiskPattern"
type: docs
weight: 1940
url: /ar/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

تمثل مجموعة تحتوي على مثيلات فئة [`RiskPattern`](../riskpattern/)

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | يحصل على مثيل فئة [`RiskPattern`](../riskpattern/) للمهمة المحددة |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | يضيف مثيلًا من فئة [`RiskPattern`](../riskpattern/) إلى هذه المجموعة |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |

## الأمثلة

يوضح كيفية العمل مع مجموعات نمط المخاطر

```csharp
var settings = new RiskAnalysisSettings
{
    // حدد عدد التكرارات لمحاكاة مونت كارلو (القيمة الافتراضية هي 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// طالما أن RiskPatternCollection ليست للقراءة فقط
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// يمكن إضافة أنماط جديدة
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// التكرار على الأنماط المضافة
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// تحرير النمط في المجموعة باستخدام الوصول عبر الفهرس
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// تحقق من الأنماط بعد التعديلات
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// يمكننا إزالة النمط
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// تحقق من عدم وجود النمط في المجموعة
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// يمكن مسح المجموعة بطريقتين

// انسخ الأنماط إلى المصفوفة واحذفها واحدة تلو الأخرى
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// أو يمكن مسح مجموعة الأنماط بالكامل
settings.Patterns.Clear();
```

### انظر أيضًا

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


