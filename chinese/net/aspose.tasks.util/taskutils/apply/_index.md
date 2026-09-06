---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUtils 方法。对树中的每个任务应用指定的算法"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

将指定算法应用于树的每个任务。

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 根 | 任务 | 树的根节点 |
| alg | ITreeAlgorithm`1 | 已应用的算法。 |
| 级别 | Int32 | 根任务的层级。 |

## 示例

展示如何使用树算法。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 收集所有项目任务
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// 将任务视为普通列表进行操作
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### 另见

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


