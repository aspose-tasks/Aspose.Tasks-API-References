---
title: "ResourceAssignment.ToString"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُعيد تمثيل نصي قصير للنسخة من فئة ResourceAssignment. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير"
type: docs
weight: 790
url: /ar/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

تُعيد تمثيل نصي قصير للنسخة من الفئة [`ResourceAssignment`](../). التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير.

```csharp
public override string ToString()
```

### قيمة الإرجاع

نص قصير يمثل كائن التعيين.

## الأمثلة

يعرض كيفية طباعة معلومات التعيين الشائعة.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


