---
title: "Project.GetPredecessors"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تُرجع مجموعة من روابط المهام التي هي سلف للمهام المحددة"
type: docs
weight: 1120
url: /ar/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

يرجع مجموعة من روابط المهام التي هي سابقة للمهمة المحددة.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | المهمة للحصول على سلفها. |

### قيمة الإرجاع

قائمة السلف [`TaskLink`](../../tasklink/).

## الأمثلة

يظهر كيفية الحصول على سلف المهمة المحددة.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// عرض أسماء مهام السلف والمتابع
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


