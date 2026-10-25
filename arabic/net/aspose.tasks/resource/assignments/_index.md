---
title: "Resource.Assignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. تحصل على مجموعة من تعيينات الموارد لهذا الكائن"
type: docs
weight: 120
url: /ar/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

يحصل على مجموعة من تعيينات الموارد لهذا الكائن.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## الأمثلة

يوضح كيفية قراءة تعيينات مورد.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### انظر أيضًا

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


