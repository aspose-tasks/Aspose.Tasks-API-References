---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 资源在其任务上已完成工作产生的费用以及与任务相关的其他记录费用."
type: docs
weight: 30
url: /zh/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

资源在其任务上已完成工作产生的费用，以及与任务相关的任何其他记录费用。

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## 示例

展示如何读取/写入 Rsc.ActualCost 属性.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


