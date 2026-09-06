---
title: "الفئة RiskPattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.RiskAnalysis.RiskPattern. تمثل نمط مخاطر لمهمة مشروع"
type: docs
weight: 1930
url: /ar/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

يمثل نمط خطر لمهمة مشروع.

```csharp
public class RiskPattern
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | ينشئ نسخة جديدة من الفئة `RiskPattern`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | يحصل أو يعيّن مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي تكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة. القيمة الافتراضية هي CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | يحصل أو يعيّن توزيع الاحتمال المستخدم في محاكاة مونت كارلو. القيمة الافتراضية هي ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | يحصل أو يعيّن النسبة المئوية لأكثر مدة محتملة للمهمة والتي يمكن أن تحدث في أفضل سيناريو ممكن للمشروع. القيمة الافتراضية هي 75، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتفائلة ستكون 3 أيام. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | يحصل أو يعيّن النسبة المئوية لأكثر مدة محتملة للمهمة والتي يمكن أن تحدث في أسوأ سيناريو ممكن للمشروع. القيمة الافتراضية هي 125، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتشائمة ستكون 5 أيام. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | يحصل على مهمة المشروع التي يُطبق عليها نمط المخاطر هذا. |

## الأمثلة

يوضح كيفية تعريف إعدادات محاكاة المخاطر.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### انظر أيضًا

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


