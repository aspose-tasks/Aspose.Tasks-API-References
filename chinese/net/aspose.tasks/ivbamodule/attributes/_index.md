---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "IVbaModule 属性。获取 VbaModuleAttributeCollection 的集合"
type: docs
weight: 10
url: /zh/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

获取 [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/) 的集合

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## 示例

展示如何读取 VBA 模块的属性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### 另见

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


