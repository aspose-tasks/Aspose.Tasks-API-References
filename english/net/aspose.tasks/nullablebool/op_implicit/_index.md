---
title: NullableBool.op_Implicit
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool method. Implicitly converts a NullableBool instance to a boolean value. Returns true when Value is true and IsDefined is true
type: docs
weight: 80
url: /net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Implicitly converts a [`NullableBool`](../) instance to a boolean value. Returns true when [`Value`](../value/) is true and [`IsDefined`](../isdefined/) is true.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | NullableBool | The value to convert. |

### Return Value

a boolean value.

## Examples

Shows how to compare &lt;see cref="Aspose.Tasks.NullableBool" /&gt; instances.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// the equality of bools is checked against to 'IsDefined' and 'Value' properties.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// checks implicit conversion to bool: bool1 is True because it is defined and Value is set to True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// checks implicit conversion to bool: bool2 is False because it is not defined.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// checks implicit conversion to bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### See Also

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## implicit operator {#op_implicit}

Implicitly converts boolean value to the [`NullableBool`](../) instance.

```csharp
public static implicit operator NullableBool(bool val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Boolean | Value to convert. |

### Return Value

Converted [`NullableBool`](../) instance.

## Examples

Shows how to compare &lt;see cref="Aspose.Tasks.NullableBool" /&gt; instances.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// the equality of bools is checked against to 'IsDefined' and 'Value' properties.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// checks implicit conversion to bool: bool1 is True because it is defined and Value is set to True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// checks implicit conversion to bool: bool2 is False because it is not defined.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// checks implicit conversion to bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### See Also

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


