---
title: "الفئة RemoveTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.RemoveTask. تزيل المهمة المحددة من شجرة المهام."
type: docs
weight: 2760
url: /ar/net/aspose.tasks.util/removetask/
---
## RemoveTask class

يزيل المهمة المحددة من شجرة المهام.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RemoveTask](removetask/)(Task) | يُنشئ مثيلاً جديداً من الفئة `RemoveTask`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | لا تفعل شيئاً. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | لا تفعل شيئاً. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | يزيل المهمة من المهمة الأصلية المحددة. |

## الأمثلة

يعرض كيفية استخدام &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt; الخوارزمية القائمة على الشجرة.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // استخدم الخوارزمية القائمة على الشجرة لحذف task1 من الشجرة
    var algorithm = new RemoveTask(task1);

    // طبق الخوارزمية على شجرة المهام
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // تحقق من النتائج
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### انظر أيضًا

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


