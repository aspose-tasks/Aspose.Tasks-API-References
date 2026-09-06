---
title: "类 VbaReference"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.VbaReference 类。表示 VbaProject 的引用。"
type: docs
weight: 2870
url: /zh/net/aspose.tasks/vbareference/
---
## VbaReference class

表示对[`VbaProject`](../vbaproject/)的引用。

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [VbaReference](vbareference/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | 获取库的标识符。 |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | 获取或设置 VBA 引用的名称。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的 `VbaReference` 对象。 |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | 返回一个值，指示此实例是否等于指定的 `VbaReference` 对象。 |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | 返回此 `VbaReference` 的哈希码值。 |

## 示例

展示如何读取 VBA 引用。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


