---
title: "Asn.CostRateTableType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。此任务使用的成本费率表"
type: docs
weight: 190
url: /zh/net/aspose.tasks/asn/costratetabletype/
---
## Asn.CostRateTableType field

此任务使用的成本费率表。

```csharp
public static readonly Key<RateType, AsnKey> CostRateTableType;
```

## 示例

展示如何读取/写入 Asn.CostRateTableType 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.CostRateTableType, RateType.B);

Console.WriteLine("Cost Rate Table Type: " + assignment.Get(Asn.CostRateTableType));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateType](../../ratetype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


