---
title: "类 ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.ChildTasksCollector 类。收集所有子任务"
type: docs
weight: 2690
url: /zh/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

收集所有子任务。

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | 初始化 `ChildTasksCollector` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | 获取收集的子对象（任务）列表。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | 处理指定的对象。 |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## 示例

展示如何将项目中的所有任务作为普通列表进行遍历。

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 另见

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


