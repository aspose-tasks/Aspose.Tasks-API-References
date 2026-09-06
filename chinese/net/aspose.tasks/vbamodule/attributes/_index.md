---
title: "VbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModule 属性。获取模块属性的集合"
type: docs
weight: 30
url: /zh/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

获取模块属性的集合。

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
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


