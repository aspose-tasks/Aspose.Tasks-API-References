---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定资源是否为空"
type: docs
weight: 420
url: /zh/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

确定资源是否为空。

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## 示例

展示如何读取/写入 Rsc.IsNull 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


