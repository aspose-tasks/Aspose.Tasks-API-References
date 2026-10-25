---
title: "الفئة ChildTasksCollector"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.ChildTasksCollector. تجمع جميع المهام الفرعية"
type: docs
weight: 2690
url: /ar/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

يجمع جميع المهام الفرعية.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | يُنشئ مثيلًا جديدًا للفئة `ChildTasksCollector`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | يحصل على قائمة بالكائنات الفرعية المجمعة (المهام). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | يعالج الكائن المحدد. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## الأمثلة

يوضح كيفية التكرار على جميع المهام في مشروع كقائمة عادية.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


