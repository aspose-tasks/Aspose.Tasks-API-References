---
title: "RemoveTask.RemoveTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ RemoveTask. يهيئ مثيلاً جديداً من الفئة RemoveTask"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/removetask/removetask/
---
## RemoveTask constructor

يهيئ مثيلاً جديداً من الفئة [`RemoveTask`](../).

```csharp
public RemoveTask(Task task)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | مهمة للإزالة. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


