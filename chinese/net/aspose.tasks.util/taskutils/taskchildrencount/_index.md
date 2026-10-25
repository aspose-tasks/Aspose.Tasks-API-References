---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUtils 方法。递归计算所有层级的任务子任务数量。"
type: docs
weight: 40
url: /zh/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

递归计算任务在所有层级的子任务数量。

```csharp
public static int TaskChildrenCount(Task task)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | 任务 | 子任务计算的任务。 |

### 返回值

子任务的数量。

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; 方法。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 递归计算任务子任务在所有层级的数量
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### 另见

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


