---
title: "Task.Assignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. يحصل على مجموعة من تعيينات الموارد لهذا الكائن"
type: docs
weight: 120
url: /ar/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

يحصل على مجموعة من تعيينات الموارد لهذا الكائن.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## الأمثلة

يُظهر كيفية التكرار على تعيينات المهمة.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // عرض تعيينات المهمة
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### انظر أيضًا

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


