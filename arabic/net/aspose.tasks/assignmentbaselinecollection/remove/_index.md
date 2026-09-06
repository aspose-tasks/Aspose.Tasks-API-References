---
title: "AssignmentBaselineCollection.Remove"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة AssignmentBaselineCollection. يزيل الخط الأساسي من هذه المجموعة"
type: docs
weight: 60
url: /ar/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

يزيل الخط الأساسي من هذه المجموعة.

```csharp
public bool Remove(AssignmentBaseline item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | AssignmentBaseline | العنصر المراد إزالته. |

### قيمة الإرجاع

صحيح إذا تم إزالة مثيل [`AssignmentBaseline`](../../assignmentbaseline/) بنجاح؛ وإلا، خطأ

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


