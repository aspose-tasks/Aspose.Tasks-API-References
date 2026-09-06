---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定资源标准成本和加班成本何时以及如何计入或累计到任务成本中"
type: docs
weight: 10
url: /zh/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

确定资源标准成本和加班成本何时以及如何计入任务成本，或计提。

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## 示例

展示如何读取/写入 Rsc.AccrueAt 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


