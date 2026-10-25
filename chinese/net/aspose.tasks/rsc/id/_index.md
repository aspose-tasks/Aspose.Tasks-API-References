---
title: "Rsc.Id"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 资源在资源列表中的位置标识符."
type: docs
weight: 350
url: /zh/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

资源在资源列表中的位置标识符。

```csharp
public static readonly Key<int, RscKey> Id;
```

## 示例

展示如何读取/写入 Rsc.Id 属性.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


