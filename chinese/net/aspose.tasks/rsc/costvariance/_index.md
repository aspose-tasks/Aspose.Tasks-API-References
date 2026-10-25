---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的基准成本与总成本之间的差额"
type: docs
weight: 250
url: /zh/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

资源的基准成本与总成本之间的差额。

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## 示例

展示如何读取/写入 Rsc.CostVariance 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


