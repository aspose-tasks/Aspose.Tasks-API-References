---
title: "Tsk.Warning"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 表示指示任务存在计划差异的标志."
type: docs
weight: 1120
url: /zh/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

表示 指示任务存在计划差异的标志。

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## 示例

展示如何读取任务警告.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


