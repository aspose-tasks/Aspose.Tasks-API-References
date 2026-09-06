---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务在资源平衡之前的完成日期"
type: docs
weight: 910
url: /zh/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

资源平衡之前任务的完成日期。

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## 示例

展示如何读取/写入 Tsk.PreleveledFinish 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


