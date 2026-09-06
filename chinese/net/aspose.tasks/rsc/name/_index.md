---
title: "Rsc.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的名称"
type: docs
weight: 460
url: /zh/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

资源的名称。

```csharp
public static readonly Key<string, RscKey> Name;
```

## 示例

展示如何读取/写入 Rsc.Name 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


