---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取指示资源是否为根资源的标志。根资源是一种特殊资源，旨在支持 MS Projects 格式的内部实现，不应直接在用户代码中使用。"
type: docs
weight: 470
url: /zh/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

获取指示资源是否为根资源的标志。根资源是一种特殊资源，旨在支持 MS Project 格式的内部实现，不应直接在用户代码中使用。

```csharp
public virtual bool IsRoot { get; }
```

## 示例

展示如何使用 IsRoot 属性跳过根资源。

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


