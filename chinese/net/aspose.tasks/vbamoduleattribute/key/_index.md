---
title: "VbaModuleAttribute.Key"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModuleAttribute 属性。获取 VBA 模块属性的键"
type: docs
weight: 10
url: /zh/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

获取 VBA 模块属性的键。

```csharp
public string Key { get; }
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


