---
title: "Task.Get"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。返回此容器中属性映射的值"
type: docs
weight: 1340
url: /zh/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

返回属性在此容器中映射的值。

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| 参数 | 描述 |
| --- | --- |
| T | 映射值的类型。 |
| key | 指定的属性键。[`Tsk`](../../tsk/) 用于获取属性键。 |

### 返回值

属性在此容器中映射的值。

## 示例

展示如何获取/设置任务属性。

```csharp
var project = new Project();

// 添加任务并设置任务属性
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


