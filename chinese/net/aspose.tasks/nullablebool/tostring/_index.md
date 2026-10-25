---
title: "NullableBool.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 方法。返回表示当前对象的字符串。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

返回表示当前对象的字符串。

```csharp
public override string ToString()
```

### 返回值

表示当前对象的字符串。

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


