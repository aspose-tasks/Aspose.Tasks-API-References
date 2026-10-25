---
title: "AssignmentBaselineCollection.Count"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية AssignmentBaselineCollection. تحصل على عدد الكائنات الموجودة في كائن AssignmentBaselineCollection هذا"
type: docs
weight: 10
url: /ar/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

يحصل على عدد الكائنات المحتواة في كائن AssignmentBaselineCollection هذا.

```csharp
public int Count { get; }
```

## الأمثلة

يوضح كيفية قراءة خطوط أساس التعيين.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// قراءة معلومات خط أساس التعيين.
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// حذف خطوط أساس التعيين
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### انظر أيضًا

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


