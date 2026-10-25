---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。材料资源的计量单位"
type: docs
weight: 440
url: /zh/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

材料资源的计量单位。

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## 示例

展示如何读取/写入 Rsc.MaterialLabel 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


