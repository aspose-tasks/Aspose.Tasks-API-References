---
title: "结构体 NullableBool"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.NullableBool 结构体。用于布尔值的类，可检查该值是否已定义"
type: docs
weight: 1110
url: /zh/net/aspose.tasks/nullablebool/
---
## NullableBool structure

用于布尔值的类，可检查该值是否已定义。

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | 使用指定的布尔值初始化 `NullableBool` 结构体的新实例。 |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | 初始化 `NullableBool` 结构体的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | 获取一个值，指示该值是否已定义；如果未定义，则为 false。 |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | 获取或设置一个值，指示当前值是 true 还是 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | 返回一个标志，指示此实例是否等于指定的 `NullableBool` 类实例。 |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | 返回一个标志，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | 返回 `NullableBool` 类实例的哈希码值。 |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | 返回表示当前对象的字符串。 |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | 隐式将 `NullableBool` 实例转换为布尔值。当 [`Value`](./value/) 为 true 且 [`IsDefined`](./isdefined/) 为 true 时返回 true。（2 个运算符） |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | 返回一个值，指示此实例是否不等于指定的对象。 |

## 示例

展示如何使用 &lt;see cref="NullableBool" /&gt; 类。

```csharp
var project = new Project();

// 让我们检查 <see cref="Aspose.Tasks.NullableBool" /> 类的使用位置
// <see cref="Aspose.Tasks.NullableBool" /> 的主要优势是 
// 可以通过构造将其设置为未定义
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// 使用可空布尔实例
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// 使用可空布尔实例
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


