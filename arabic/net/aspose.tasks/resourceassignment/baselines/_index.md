---
title: "ResourceAssignment.Baselines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceAssignment. يحصل على كائن AssignmentBaselineCollection. مجموعة قيم الخط الأساسي المرتبطة بالتعيين"
type: docs
weight: 120
url: /ar/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

يحصل على كائن AssignmentBaselineCollection. مجموعة قيم الخط الأساسي المرتبطة بتعيين.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## الأمثلة

يظهر كيفية الوصول إلى الخطوط الأساسية للتعيين.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### انظر أيضًا

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


