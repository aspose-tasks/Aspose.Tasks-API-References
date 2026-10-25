---
title: "الفئة RiskItemStatistics"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.RiskAnalysis.RiskItemStatistics. تمثل عنصرًا يخزن البيانات الإحصائية لمهمة المشروع المُحلَّل"
type: docs
weight: 1900
url: /ar/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

يمثل عنصرًا يخزن البيانات الإحصائية للمهمة في المشروع المُحلل.

```csharp
public class RiskItemStatistics
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | يحصل على القيمة المتوقعة لعنصر المخاطر. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | يحصل على نسخة من تعداد [`RiskItemType`](../riskitemtype/). |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | يحصل على القيمة القصوى التي تم توليدها أثناء محاكاة مونت كارلو. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | يحصل على القيمة الدنيا التي تم توليدها أثناء محاكاة مونت كارلو. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | يحصل على الانحراف المعياري لعنصر المخاطر. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | يحصل على قيمة يكون أقل منها النسبة المئوية المحددة من العينات المولدة. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | يعيد تمثيلًا نصيًا قصيرًا لعنصر المخاطر. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير. |

## الأمثلة

يوضح كيفية حساب إحصائيات المخاطر.

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

// تحليل مخاطر المشروع
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### انظر أيضًا

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


