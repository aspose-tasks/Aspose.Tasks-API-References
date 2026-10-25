---
title: "Rsc.Code"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的代码或其他信息"
type: docs
weight: 210
url: /zh/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

资源的代码或其他信息。

```csharp
public static readonly Key<string, RscKey> Code;
```

## 示例

展示如何读取/写入 Rsc.Code 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


