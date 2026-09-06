---
title: "Rsc.Initials"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 资源的缩写."
type: docs
weight: 370
url: /zh/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

资源的首字母缩写。

```csharp
public static readonly Key<string, RscKey> Initials;
```

## 示例

展示如何读取/写入 Rsc.Initials 属性.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


