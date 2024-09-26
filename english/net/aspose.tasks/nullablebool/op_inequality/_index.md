---
title: NullableBool.op_Inequality
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool method. Returns a value indicating whether this instance is not equal to a specified object
type: docs
weight: 90
url: /net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

Returns a value indicating whether this instance is not equal to a specified object.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| Parameter | Type | Description |
| --- | --- | --- |
| a | NullableBool | The first [`NullableBool`](../). |
| b | NullableBool | The second [`NullableBool`](../). |

### Return Value

a value indicating whether this instance is not equal to a specified object

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


