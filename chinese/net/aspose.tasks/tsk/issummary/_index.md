---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否为汇总任务"
type: docs
weight: 720
url: /zh/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

确定任务是否为汇总任务。

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## 示例

展示如何读取/写入 Tsk.IsSummary 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


