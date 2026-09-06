---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定固定成本的计费或计入任务成本的时间和方式"
type: docs
weight: 440
url: /zh/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

确定固定成本何时以及如何计入任务成本的选项。

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## 示例

展示如何读取/写入 Tsk.FixedCostAccrual 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


