---
title: "TaskBaselineCollection.Remove"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskBaselineCollection. تزيل الخط الأساسي من هذه المجموعة"
type: docs
weight: 50
url: /ar/net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

يزيل الخط الأساسي من هذه المجموعة.

```csharp
public bool Remove(TaskBaseline item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | TaskBaseline | العنصر المراد إزالته. |

### قيمة الإرجاع

صحيح إذا تم إزالة العنصر بنجاح؛ وإلا، خطأ

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


