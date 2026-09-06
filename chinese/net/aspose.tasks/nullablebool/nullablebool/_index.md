---
title: "NullableBool.NullableBool"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 构造函数。使用指定的布尔值初始化 NullableBool 结构的新实例。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

使用指定的布尔值初始化 [`NullableBool`](../) 结构的新实例。

```csharp
public NullableBool(bool value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | Boolean | 指定的布尔值。 |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## NullableBool(bool, bool) {#constructor_1}

初始化一个新的 [`NullableBool`](../) 结构体实例。

```csharp
public NullableBool(bool value, bool isDefined)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | Boolean | 当前值。 |
| isDefined | Boolean | 指示当前值是否已定义的值。 |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


