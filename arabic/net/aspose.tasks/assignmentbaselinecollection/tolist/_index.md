---
title: "AssignmentBaselineCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة AssignmentBaselineCollection. تحول كائن AssignmentBaselineCollection إلى قائمة من كائنات AssignmentBaseline"
type: docs
weight: 70
url: /ar/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

تحول كائن AssignmentBaselineCollection إلى قائمة من كائنات [`AssignmentBaseline`](../../assignmentbaseline/) .

```csharp
public List<AssignmentBaseline> ToList()
```

### قيمة الإرجاع

قائمة من كائنات [`AssignmentBaseline`](../../assignmentbaseline/) .

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


