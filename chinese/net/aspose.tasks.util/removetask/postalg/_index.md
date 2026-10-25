---
title: "RemoveTask.PostAlg"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RemoveTask 方法。什么也不做"
type: docs
weight: 30
url: /zh/net/aspose.tasks.util/removetask/postalg/
---
## RemoveTask.PostAlg method

不执行任何操作。

```csharp
public void PostAlg(Task el, int level)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | 任务 | 要处理的对象。 |
| 级别 | Int32 | 树节点层级。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt; 基于树的算法。

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

    // 使用基于树的算法从树中删除 task1
    var algorithm = new RemoveTask(task1);

    // 将算法应用于任务树
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // 检查结果
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### 另见

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


