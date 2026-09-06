---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定调平功能是否可以延迟并拆分单个分配，以解决资源过度分配。"
type: docs
weight: 750
url: /zh/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

确定平衡功能是否可以延迟并拆分单个任务分配，以解决资源超额分配。

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## 示例

展示如何读取/写入 Tsk.LevelAssignments 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


