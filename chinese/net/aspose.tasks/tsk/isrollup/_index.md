---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定是否将子任务甘特条的信息汇总到汇总任务条。"
type: docs
weight: 690
url: /zh/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

确定子任务甘特条的信息是否会汇总到汇总任务条中。

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## 示例

展示如何读取/写入 Tsk.IsRollup 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


