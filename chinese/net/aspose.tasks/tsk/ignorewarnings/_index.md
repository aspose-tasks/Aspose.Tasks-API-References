---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。指示是否在 Microsoft Project 中隐藏调度冲突警告指示器"
type: docs
weight: 540
url: /zh/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

指示是否在 Microsoft Project 中隐藏日程冲突警告指示器。

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## 示例

展示如何读取/写入 Tsk.IgnoreWarnings 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


