---
title: "类 TaskUtils"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.TaskUtils 类。提供任务有用操作的辅助类"
type: docs
weight: 2770
url: /zh/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

提供对任务有用操作的辅助类。

```csharp
public static class TaskUtils
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | 将指定算法应用于树的每个任务。 |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | 构建满足条件的任务新树。 |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | 在任务树中查找满足条件的任务。 |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | 递归计算任务在所有层级的子任务数量。 |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


