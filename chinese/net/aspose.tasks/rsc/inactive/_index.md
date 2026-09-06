---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定资源是否被具有管理员权限的用户设为非活动"
type: docs
weight: 360
url: /zh/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

确定资源是否被具有管理员权限的用户设为非活动状态。

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## 示例

展示如何读取/写入 Rsc.Inactive 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


