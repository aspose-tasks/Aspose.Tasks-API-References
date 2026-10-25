---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。指示资源产生的成本应计入的成本中心"
type: docs
weight: 230
url: /zh/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

指示资源产生的成本应计入的成本中心。

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## 示例

展示如何读取/写入 Rsc.CostCenter 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


