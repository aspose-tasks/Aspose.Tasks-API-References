---
title: "Rsc.Hyperlink"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。与资源关联的超链接的标题或说明文字"
type: docs
weight: 320
url: /zh/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

与资源关联的超链接的标题或说明文字。

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

## 示例

展示如何读取/写入 资源的超链接属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


