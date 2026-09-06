---
title: "类 VbaModuleAttribute"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaModuleAttribute 类。VbaModule 对象的属性。"
type: docs
weight: 2820
url: /zh/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

[`VbaModule`](../vbamodule/) 对象的属性。

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | 获取 VBA 模块属性的键。 |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | 获取 VBA 模块属性的值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的 `VbaModuleAttribute` 对象。 |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | 返回一个值，指示此实例是否等于指定的 `VbaModuleAttribute` 对象。 |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | 返回此 `VbaModuleAttribute` 的哈希码值。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


