---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。可用作计算已完成工作预算成本（BCWP）的替代的完成百分比值"
type: docs
weight: 900
url: /zh/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

可用作计算已完成工作预算成本（BCWP）的替代值的完成百分比。

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## 示例

展示如何读取/写入 Tsk.PhysicalPercentComplete 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


