---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否手动调度"
type: docs
weight: 610
url: /zh/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

确定任务是否为手动调度。

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## 示例

展示如何读取/写入 Tsk.IsManual 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


