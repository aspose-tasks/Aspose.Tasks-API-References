---
title: "RiskItemStatisticsCollection.Get"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة RiskItemStatisticsCollection. تُرجع نسخة من فئة RiskItemStatistics الموجودة في هذه المجموعة والمرتبطة بكائن Task المحدد، أو null إذا لم يتم العثور على العنصر."
type: docs
weight: 10
url: /ar/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/get/
---
## RiskItemStatisticsCollection.Get method

تُرجع نسخة من فئة [`RiskItemStatistics`](../../riskitemstatistics/) الموجودة في هذه المجموعة والمرتبطة بكائن Task المحدد؛ null إذا لم يتم العثور على العنصر.

```csharp
public RiskItemStatistics Get(Task task)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| task | Task | النُسخة المحددة من فئة [`Task`](../../../aspose.tasks/task/). |

### قيمة الإرجاع

عنصر المخاطر المرتبط بكائن المهمة المحدد إذا تم العثور عليه؛ وإلا null.

## الأمثلة

يوضح كيفية العمل مع مجموعة إحصاءات المخاطر.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// تهيئة نمط المخاطر
var pattern = new RiskPattern(task)
{
    // اختر نوع التوزيع لمولد الأعداد العشوائية لتوليد القيم الممكنة منه (يدعم حاليًا نوعان فقط، وهما الطبيعي والموحد)
    // لمزيد من التفاصيل راجع هنا: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // حدد النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو ممكن للمشروع
    // القيمة الافتراضية هي 75، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتفائلة ستكون 3 أيام
    Optimistic = 70,

    // حدد النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو ممكن للمشروع
    // القيمة الافتراضية هي 125، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتشائمة ستكون 5 أيام.
    Pessimistic = 130,

    // حدد مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم الفعلية ضمن التقديرات المتفائلة والمتشائمة.
    // يمكنك التفكير فيه كقيمة للانحراف المعياري: كلما زادت عدم اليقين في تقديراتك، زادت قيمة الانحراف المعياري المستخدمة في مولد الأعداد العشوائية.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// التكرار عبر جميع عناصر الإحصاءات
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// أو الحصول على إحصائية محددة
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### انظر أيضًا

* class [RiskItemStatistics](../../riskitemstatistics/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskItemStatisticsCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatisticscollection/)
* assembly [Aspose.Tasks](../../../)


