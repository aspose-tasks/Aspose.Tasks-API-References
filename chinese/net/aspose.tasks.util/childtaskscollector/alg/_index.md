---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ChildTasksCollector 方法。处理指定的对象"
type: docs
weight: 30
url: /zh/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

处理指定的对象。

```csharp
public override void Alg(Task el, int level)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | 任务 | 要处理的对象。 |
| 级别 | Int32 | 树节点层级。 |

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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


