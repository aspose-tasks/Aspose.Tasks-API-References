---
title: "الفئة TaskUtils"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.TaskUtils. فئة مساعدة توفر عمليات مفيدة مع المهام"
type: docs
weight: 2770
url: /ar/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

فئة مساعدة توفر عمليات مفيدة مع المهام.

```csharp
public static class TaskUtils
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | يطبق الخوارزمية المحددة على كل مهمة في شجرة. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | يبني شجرة جديدة من المهام التي تستوفي الشرط. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | يجد مهمة تستوفي الشرط في شجرة المهام. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | يحسب بشكل متكرر عدد مهام الأطفال لمهمة عبر جميع المستويات. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


