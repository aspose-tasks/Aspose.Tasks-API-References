---
title: "RiskPatternCollection.Contains"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة RiskPatternCollection. تُرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة وإلا false"
type: docs
weight: 60
url: /ar/net/aspose.tasks.riskanalysis/riskpatterncollection/contains/
---
## RiskPatternCollection.Contains method

يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.

```csharp
public bool Contains(RiskPattern item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | RiskPattern | العنصر المحدد للبحث عنه. |

### قيمة الإرجاع

صحيح إذا وُجد العنصر المحدد في هذه المجموعة؛ وإلا، خطأ.

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

* class [RiskPattern](../../riskpattern/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


