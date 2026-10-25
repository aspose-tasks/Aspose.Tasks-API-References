---
title: "Tsk.Type"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的类型"
type: docs
weight: 1100
url: /zh/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

任务的类型。

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## 示例

展示如何读取/写入 Tsk.Type 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


