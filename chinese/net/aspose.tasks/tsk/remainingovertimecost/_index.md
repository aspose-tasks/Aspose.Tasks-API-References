---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务剩余的计划加班费用"
type: docs
weight: 970
url: /zh/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

任务剩余的计划加班费用。

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## 示例

展示如何读取/写入 Tsk.RemainingOvertimeCost 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


