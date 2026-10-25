---
title: "NullableBool.op_Implicit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 方法。隐式将 NullableBool 实例转换为布尔值。当 Value 为 true 且 IsDefined 为 true 时返回 true"
type: docs
weight: 80
url: /zh/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

隐式将 [`NullableBool`](../) 实例转换为布尔值。当 [`Value`](../value/) 为 true 且 [`IsDefined`](../isdefined/) 为 true 时返回 true。

```csharp
public static implicit operator bool(NullableBool val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | NullableBool | 要转换的值。 |

### 返回值

布尔值。

## 示例

展示如何比较 &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt; 实例。

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool 的相等性是针对 'IsDefined' 和 'Value' 属性进行检查的。
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// 检查隐式转换为 bool：bool1 为 True，因为它已定义且 Value 被设置为 True。
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// 检查隐式转换为 bool：bool2 为 False，因为它未定义。
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// 检查隐式转换为 bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### 另见

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## implicit operator {#op_implicit}

隐式将布尔值转换为 [`NullableBool`](../) 实例。

```csharp
public static implicit operator NullableBool(bool val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | Boolean | 要转换的值。 |

### 返回值

已转换的 [`NullableBool`](../) 实例。

## 示例

展示如何比较 &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt; 实例。

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool 的相等性是针对 'IsDefined' 和 'Value' 属性进行检查的。
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// 检查隐式转换为 bool：bool1 为 True，因为它已定义且 Value 被设置为 True。
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// 检查隐式转换为 bool：bool2 为 False，因为它未定义。
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// 检查隐式转换为 bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### 另见

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


