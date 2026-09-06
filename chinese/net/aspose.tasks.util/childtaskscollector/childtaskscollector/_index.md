---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ChildTasksCollector 构造函数。初始化 ChildTasksCollector 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

初始化 [`ChildTasksCollector`](../) 类的新实例。

```csharp
public ChildTasksCollector()
```

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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


