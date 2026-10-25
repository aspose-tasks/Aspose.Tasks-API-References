---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定资源是否为通用"
type: docs
weight: 410
url: /zh/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

确定资源是否为通用资源。

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## 示例

展示如何读取/写入 Rsc.IsGeneric 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


