---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。已由指派资源在任务上完成的加班工作产生的费用"
type: docs
weight: 50
url: /zh/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

指派资源在任务上已完成的加班工作产生的费用。

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## 示例

展示如何读取/写入 Tsk.ActualOvertimeCost 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


