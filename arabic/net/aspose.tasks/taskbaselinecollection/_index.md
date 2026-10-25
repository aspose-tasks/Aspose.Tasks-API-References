---
title: "الفئة TaskBaselineCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskBaselineCollection. تمثل مجموعة من كائنات TaskBaseline"
type: docs
weight: 2380
url: /ar/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

يمثل مجموعة من كائنات [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في كائن TaskBaselineCollection هذا. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | يزيل الخط الأساسي من هذه المجموعة. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | يحوّل كائن TaskBaselineCollection إلى قائمة من كائنات [`TaskBaseline`](../taskbaseline/). |

## الأمثلة

يوضح كيفية العمل مع مجموعات الخط الأساسي للمهمة.

```csharp
var project = new Project();

// إنشاء خطوط أساسية للمشروع
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// طباعة خطوط أساسية للمهمة
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// لنقم بمسح جميع الخطوط الأساسية
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### انظر أيضًا

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


