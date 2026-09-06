---
title: "Task.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُرجع قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لمهمة محددة"
type: docs
weight: 1330
url: /ar/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

يرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لمهمة محددة.

```csharp
public bool Equals(Task other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | مهمة | المهمة المحددة للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُرجع true إذا كانت المهمة المحددة وهذه المثيلة لها معرّفات فريدة متساوية.

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن المحدد للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُرجع true إذا كانت المهمة المحددة وهذه المثيلة لها معرّفات فريدة متساوية.

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


