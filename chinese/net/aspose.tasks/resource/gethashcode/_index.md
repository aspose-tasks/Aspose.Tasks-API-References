---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 方法。返回 Resource 类实例的哈希码值"
type: docs
weight: 840
url: /zh/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

返回 [`Resource`](../) 类实例的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取资源的哈希码。

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// 资源的哈希码等于资源 UID
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


