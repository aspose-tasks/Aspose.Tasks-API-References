---
title: "الفئة AssignmentBaseline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.AssignmentBaseline. تمثل Baseline لتعيين مورد"
type: docs
weight: 50
url: /ar/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

يمثل الخط الأساسي لتخصيص المورد.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | يحصل أو يعيّن الرقم الفريد لسجل بيانات الخط الأساسي. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | يحصل أو يعيّن التكلفة الموازنة للعمل الذي أُجري بواسطة مورد لمشروع حتى الآن. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | يحصل أو يعيّن تكلفة الميزانية للعمل المجدول لمورد. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | يحصل أو يعيّن التكلفة المتوقعة لمورد عندما يتم حفظ الخط الأساسي. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | يحصل أو يعيّن تاريخ الانتهاء المجدول لتعيين المورد عندما تم حفظ الخط الأساسي. تاريخ الانتهاء لتعيين المورد عندما تم حفظ هذا الخط الأساسي. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | يحصل أو يعيّن تاريخ البدء المجدول لتعيين المورد عندما تم حفظ الخط الأساسي. تاريخ البدء لتعيين المورد عندما تم حفظ هذا الخط الأساسي. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | يحصل أو يعيّن كائن [`TimephasedDataCollection`](../timephaseddatacollection/) لهذا الكائن. البيانات الزمنية المرتبطة بخط أساس تعيين المورد. تُعيد كائن [`TimephasedDataCollection`](../timephaseddatacollection/) لهذا الكائن. مجموعة البيانات الزمنية المرتبطة بهذا الخط الأساسي. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | يحصل أو يعيّن العمل المخصص لمورد عندما يتم حفظ الخط الأساسي. كمية العمل المخصص لمورد عندما تم حفظ الخط الأساسي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | تنفيذ واجهة IComparable. يقارن هذه الحالة بالكائن Baseline المحدد. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | تنفيذ واجهة IComparable. يقارن هذه الحالة بالكائن Baseline المحدد. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية للكيان AssignmentBaseline المحدد. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## الأمثلة

يظهر كيفية العمل مع خطوط أساس التعيينات.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// يتم تعيين خطوط أساس التعيينات عندما يتم تعيين الخط الأساسي للمشروع بالكامل.
project.SetBaseline(BaselineType.Baseline);

// قراءة معلومات خط أساس التعيين.
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// تحقق من مساواة الخط الأساسي.
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// يمكن مقارنة الخطوط الأساسية باستخدام تحميلات طريقة 'Equals'.
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// أو باستخدام عملية حسابية محملة.
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// رمز التجزئة للخط الأساسي يعتمد على رقم الخط الأساسي.
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### انظر أيضًا

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


