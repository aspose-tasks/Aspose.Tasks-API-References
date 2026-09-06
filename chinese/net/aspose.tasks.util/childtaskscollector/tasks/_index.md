---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ChildTasksCollector 属性。获取收集的子对象任务列表"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

获取收集的子对象（任务）列表。

```csharp
public List<Task> Tasks { get; }
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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


