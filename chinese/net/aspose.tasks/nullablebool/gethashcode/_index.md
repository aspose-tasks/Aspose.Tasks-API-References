---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 方法。返回 NullableBool 类实例的哈希码值。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

返回 [`NullableBool`](../) 类实例的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode 方法。

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// 布尔值的哈希码基于 'IsDefined' 和 'Value' 属性。
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### 另见

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


