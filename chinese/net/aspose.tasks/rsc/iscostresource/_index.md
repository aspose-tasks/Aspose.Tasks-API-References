---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定资源是否为成本资源"
type: docs
weight: 390
url: /zh/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

确定资源是否为成本资源。

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## 示例

展示如何读取/写入 Rsc.IsCostResource 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


