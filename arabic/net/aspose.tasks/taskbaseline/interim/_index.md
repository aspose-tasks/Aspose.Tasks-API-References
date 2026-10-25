---
title: "TaskBaseline.Interim"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskBaseline. يحصل أو يضبط قيمة تشير إلى ما إذا كان هذا خط أساس مؤقت"
type: docs
weight: 60
url: /ar/net/aspose.tasks/taskbaseline/interim/
---
## TaskBaseline.Interim property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا.

```csharp
public bool Interim { get; set; }
```

## الأمثلة

يوضح كيفية الوصول إلى معلومات الخط الأساسي.

```csharp
var project = new Project();

// إنشاء TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// عرض مدة الخط الأساسي للمهمة
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// طباعة البيانات الزمنية للخط الأساسي للمهمة
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### انظر أيضًا

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


