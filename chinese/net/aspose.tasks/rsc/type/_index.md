---
title: "Rsc.Type"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的类型"
type: docs
weight: 660
url: /zh/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

资源的类型。

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## 示例

展示如何读取/写入 Rsc.Type 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


