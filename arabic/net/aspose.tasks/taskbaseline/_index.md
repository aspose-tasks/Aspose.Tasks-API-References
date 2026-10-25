---
title: "فئة TaskBaseline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.TaskBaseline. تمثل الخط الأساسي لمهمة."
type: docs
weight: 2370
url: /ar/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

يمثّل الخط الأساسي لمهمة.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | يُهيئ نسخة جديدة من الفئة `TaskBaseline`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | يحصل أو يعيّن الرقم الفريد لسجل بيانات الخط الأساسي. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | يحصل أو يعيّن التكلفة الموازنة للعمل الذي أُجري بواسطة مورد لمشروع حتى الآن. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | يحصل أو يعيّن تكلفة الميزانية للعمل المجدول لمورد. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | يحصل أو يعيّن التكلفة المتوقعة لمورد عندما يتم حفظ الخط الأساسي. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | يحصل أو يعيّن المدة المجدولة للمهمة عندما تم حفظ الخط الأساسي. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت مدة الخط الأساسي للمهمة مقدرة. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | يحصل أو يعيّن تاريخ الانتهاء المجدول للمهمة عندما تم حفظ الخط الأساسي. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | يحصل أو يعيّن تكلفة ثابتة للمهمة عندما تم حفظ الخط الأساسي. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان هذا خطًا أساسيًا مؤقتًا. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | يحصل أو يعيّن تاريخ البدء المجدول للمهمة عندما تم حفظ الخط الأساسي. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | يحصل أو يعيّن كائنًا من نوع TimephasedDataCollection لهذا الكائن. البيانات الزمنية المرتبطة بالخط الأساسي للمهمة. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | يحصل أو يعيّن العمل المخصص لمورد عندما يتم حفظ الخط الأساسي. كمية العمل المخصص لمورد عندما تم حفظ الخط الأساسي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | تنفيذ واجهة IComparable. يقارن هذه الحالة بالكائن Baseline المحدد. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | تنفيذ واجهة IComparable. يقارن هذه الحالة بالكائن Baseline المحدد. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | يرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن `TaskBaseline` المحدد. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | يرجع قيمة رمز تجزئة للنسخة من الفئة `TaskBaseline`. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


