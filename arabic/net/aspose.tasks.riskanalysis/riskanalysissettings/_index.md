---
title: "الفئة RiskAnalysisSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings. تحدد الإعدادات لإجراء تحليل المخاطر."
type: docs
weight: 1880
url: /ar/net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

يحدد الإعدادات لإجراء تحليل المخاطر.

```csharp
public class RiskAnalysisSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | يقوم بتهيئة نسخة جديدة من الفئة `RiskAnalysisSettings`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | يحصل أو يضبط عدد التكرارات المستخدمة في محاكاة مونت كارلو. القيمة الافتراضية هي 100. |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | يحصل على مجموعة تحتوي على نسخ الفئة [`RiskPattern`](../riskpattern/). |

## الأمثلة

يوضح كيفية إعداد إعدادات تحليل المخاطر لمحاكيات مونت كارلو.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// حدد عدد التكرارات لمحاكاة مونت كارلو (القيمة الافتراضية هي 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// تهيئة نمط المخاطر
var pattern = new RiskPattern(task);

// اختر نوع التوزيع لمولد الأعداد العشوائية لتوليد القيم الممكنة منه (يدعم حاليًا نوعان فقط، وهما الطبيعي والموحد)
// لمزيد من التفاصيل راجع هنا: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// حدد النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو ممكن للمشروع
// القيمة الافتراضية هي 75، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتفائلة ستكون 3 أيام
pattern.Optimistic = 70;

// حدد النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو ممكن للمشروع
// القيمة الافتراضية هي 125، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتشائمة ستكون 5 أيام.
pattern.Pessimistic = 130;

// حدد مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم الفعلية ضمن التقديرات المتفائلة والمتشائمة.
// يمكنك التفكير فيه كقيمة للانحراف المعياري: كلما زادت عدم اليقين في تقديراتك، زادت قيمة الانحراف المعياري المستخدمة في مولد الأعداد العشوائية.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### انظر أيضًا

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


