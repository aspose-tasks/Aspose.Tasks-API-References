---
title: "Rsc.Guid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。包含为资源生成的唯一标识代码"
type: docs
weight: 310
url: /zh/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

包含为资源生成的唯一标识代码。

```csharp
public static readonly Key<string, RscKey> Guid;
```

## 示例

展示如何读取/写入 Rsc.Guid 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


