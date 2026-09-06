---
title: "NullableBool.op_Equality"
second_title: "Aspose.Tasks for .NET API 参考"
description: "NullableBool 方法。返回一个值，指示此实例是否等于指定的对象。"
type: docs
weight: 70
url: /zh/net/aspose.tasks/nullablebool/op_equality/
---
## NullableBool Equality operator

返回一个值，指示此实例是否等于指定的对象。

```csharp
public static bool operator ==(NullableBool a, NullableBool b)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | NullableBool | 第一个 [`NullableBool`](../)。 |
| b | NullableBool | 第二个 [`NullableBool`](../)。 |

### 返回值

一个指示此实例是否等于指定对象的值。

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


