---
title: "ChildTasksCollector.Alg"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ChildTasksCollector. تعالج الكائن المحدد"
type: docs
weight: 30
url: /ar/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

يعالج الكائن المحدد.

```csharp
public override void Alg(Task el, int level)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | مهمة | الكائن للمعالجة. |
| المستوى | Int32 | مستوى عقدة الشجرة. |

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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


