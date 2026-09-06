---
title: "NullableBool.IsDefined"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 属性。获取一个值，指示该值是否已定义，否则为 false。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

获取一个值，指示该值是否已定义；如果未定义，则为 false。

```csharp
public bool IsDefined { get; }
```

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


