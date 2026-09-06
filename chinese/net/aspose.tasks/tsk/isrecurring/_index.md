---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否属于一系列循环任务"
type: docs
weight: 670
url: /zh/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

确定任务是否是循环任务系列的一部分。

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## 示例

展示如何读取/写入 Tsk.IsRecurring 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


