---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定是否可以对资源进行资源平衡"
type: docs
weight: 200
url: /zh/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

确定是否可以对资源进行资源平衡。

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## 示例

展示如何读取/写入 Rsc.CanLevel 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


