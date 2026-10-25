---
title: "RiskAnalysisResult.SaveReport"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة RiskAnalysisResult. تحفظ تقرير تحليل المخاطر إلى التدفق بصيغة PDF"
type: docs
weight: 20
url: /ar/net/aspose.tasks.riskanalysis/riskanalysisresult/savereport/
---
## SaveReport(Stream) {#savereport}

يحفظ تقرير تحليل المخاطر إلى الدفق بصيغة PDF.

```csharp
public void SaveReport(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | التدفق لحفظ تقرير تحليل المخاطر إليه. |

## الأمثلة

يوضح كيفية حساب إحصاءات المخاطر وحفظها كملف تقرير PDF.

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

// احفظ التحليل كتقرير في ملف عبر مسار الملف
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// أو احفظ التحليل إلى دفق
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### انظر أيضًا

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_1}

يحفظ تقرير تحليل المخاطر إلى مسار الملف المحدد بصيغة PDF.

```csharp
public void SaveReport(string fileName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fileName | سلسلة | اسم الملف المحدد. |

## الأمثلة

يوضح كيفية حساب إحصاءات المخاطر وحفظها كملف تقرير PDF.

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

// احفظ التحليل كتقرير في ملف عبر مسار الملف
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// أو احفظ التحليل إلى دفق
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### انظر أيضًا

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)


