---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。每次使用资源时产生的费用"
type: docs
weight: 240
url: /zh/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

每次使用资源时产生的成本。

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## 示例

展示如何读取/写入 Rsc.CostPerUse 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


