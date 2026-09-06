---
title: "类 RemoveTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.RemoveTask 类。将指定任务从任务树中移除"
type: docs
weight: 2760
url: /zh/net/aspose.tasks.util/removetask/
---
## RemoveTask class

从任务树中移除指定的任务。

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RemoveTask](removetask/)(Task) | 初始化 `RemoveTask` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | 不执行任何操作。 |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | 不执行任何操作。 |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | 从指定的父任务中移除该任务。 |

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

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


