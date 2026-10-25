---
title: "TaskUtils.Apply"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskUtils. تطبق الخوارزمية المحددة على كل مهمة في شجرة."
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

يطبق الخوارزمية المحددة على كل مهمة في شجرة.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| جذر | مهمة | جذر الشجرة |
| alg | ITreeAlgorithm`1 | الخوارزمية المطبقة. |
| المستوى | Int32 | مستوى مهمة الجذر. |

## الأمثلة

يظهر كيفية العمل مع خوارزمية شجرة.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// جمع جميع مهام المشروع
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// العمل مع المهام كما مع قائمة عادية
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


