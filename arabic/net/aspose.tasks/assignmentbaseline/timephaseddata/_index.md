---
title: "AssignmentBaseline.TimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية AssignmentBaseline. يحصل أو يحدد مثيل TimephasedDataCollection لهذا الكائن. البيانات المرحلية المرتبطة بخط أساس تعيين المورد. يرجع مثيل TimephasedDataCollection لهذا الكائن. مجموعة البيانات المرحلية المرتبطة بهذا الخط الأساسي"
type: docs
weight: 40
url: /ar/net/aspose.tasks/assignmentbaseline/timephaseddata/
---
## AssignmentBaseline.TimephasedData property

يحصل أو يحدد مثيل [`TimephasedDataCollection`](../../timephaseddatacollection/) لهذا الكائن. البيانات المرحلية المرتبطة بخط أساس تعيين المورد. يرجع مثيل [`TimephasedDataCollection`](../../timephaseddatacollection/) لهذا الكائن. مجموعة البيانات المرحلية المرتبطة بهذا الخط الأساسي.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


