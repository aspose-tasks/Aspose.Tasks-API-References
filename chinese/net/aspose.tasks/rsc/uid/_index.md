---
title: "Rsc.Uid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的唯一标识符"
type: docs
weight: 670
url: /zh/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

资源的唯一标识符。

```csharp
public static readonly Key<int, RscKey> Uid;
```

## 示例

展示如何读取/写入 Rsc.Uid 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


