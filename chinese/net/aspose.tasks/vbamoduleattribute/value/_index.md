---
title: "VbaModuleAttribute.Value"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModuleAttribute 属性。获取 VBA 模块属性的值"
type: docs
weight: 20
url: /zh/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

获取 VBA 模块属性的值。

```csharp
public string Value { get; }
```

## 示例

展示如何使用 VBA 模块属性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### 另见

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


