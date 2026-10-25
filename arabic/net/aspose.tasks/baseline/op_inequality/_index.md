---
title: "Baseline.op_Inequality"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Baseline. تُرجع قيمة تشير إلى ما إذا كانت هذه المثيلة ليست مساوية لكائن محدد"
type: docs
weight: 130
url: /ar/net/aspose.tasks/baseline/op_inequality/
---
## Baseline Inequality operator

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد.

```csharp
public static bool operator !=(Baseline a, Baseline b)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| a | Baseline | الخط الأساسي الأول. |
| b | Baseline | الخط الأساسي الثاني. |

### قيمة الإرجاع

قيمة تشير إلى ما إذا كانت هذه المثيلة غير مساوية لكائن محدد

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


