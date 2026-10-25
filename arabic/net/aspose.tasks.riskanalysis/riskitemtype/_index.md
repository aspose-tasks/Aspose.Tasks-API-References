---
title: "التعداد RiskItemType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.RiskAnalysis.RiskItemType. يحدد حقول المهمة التي يتم جمع المعلومات الإحصائية عنها أثناء تحليل المخاطر."
type: docs
weight: 1920
url: /ar/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

يحدد حقول المهمة التي يتم جمع المعلومات الإحصائية لها أثناء تحليل المخاطر.

```csharp
public enum RiskItemType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Start | `0` | بدء المهمة. |
| Finish | `1` | إنهاء المهمة. |
| EarlyStart | `2` | بدء مبكر للمهمة. |
| EarlyFinish | `3` | إنهاء مبكر للمهمة. |
| LateStart | `4` | بدء متأخر للمهمة. |
| LateFinish | `5` | إنهاء متأخر للمهمة. |

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

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


