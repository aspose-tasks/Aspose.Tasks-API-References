---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。显示资源是来自企业资源池（true）还是本地资源池（false）"
type: docs
weight: 400
url: /zh/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

显示资源是来自企业资源池（true）还是本地资源池（false）。

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## 示例

展示如何读取/写入 Rsc.IsEnterprise 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


