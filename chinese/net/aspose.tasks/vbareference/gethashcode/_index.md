---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaReference 方法。返回此 VbaReference 的哈希码值"
type: docs
weight: 50
url: /zh/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

返回此 [`VbaReference`](../) 的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取 VBA 引用的哈希码。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 引用的哈希码是内部引用 GUID 的哈希码
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### 另见

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


