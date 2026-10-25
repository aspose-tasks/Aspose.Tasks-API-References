---
title: "Task.Baselines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Task property. يحصل أو يعيّن مجموعة قيم الخط الأساسي للمهمة"
type: docs
weight: 130
url: /ar/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

يحصل أو يعيّن مجموعة قيم الخط الأساسي للمهمة.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## الأمثلة

يظهر كيفية قراءة الخطوط الأساسية للـ task.

```csharp
var project = new Project();

// تعيين خط أساس
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// عرض مدة الخط الأساسي للمهمة
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### انظر أيضًا

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


