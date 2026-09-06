---
title: "فئة AssignmentBaselineCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.AssignmentBaselineCollection. تمثل مجموعة من كائنات AssignmentBaseline"
type: docs
weight: 60
url: /ar/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

يمثل مجموعة من كائنات [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | يحصل على عدد الكائنات المحتواة في كائن AssignmentBaselineCollection هذا. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | يحصل على العنصر الأب [`ResourceAssignment`](../resourceassignment/) لهذه المجموعة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | يزيل الخط الأساسي من هذه المجموعة. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | يحوّل كائن AssignmentBaselineCollection إلى قائمة من كائنات [`AssignmentBaseline`](../assignmentbaseline/). |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


