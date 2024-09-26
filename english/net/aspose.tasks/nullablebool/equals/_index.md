---
title: NullableBool.Equals
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool method. Returns a flag indicating whether this instance is equal to the specified instance of the NullableBool class
type: docs
weight: 40
url: /net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Returns a flag indicating whether this instance is equal to the specified instance of the [`NullableBool`](../) class.

```csharp
public bool Equals(NullableBool other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | NullableBool | the specified object to compare to this instance. |

### Return Value

a flag indicating whether this instance is equal to the specified instance of the [`NullableBool`](../) class.

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

## Equals(object) {#equals_1}

Returns a flag indicating whether this instance is equal to the specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | the specified object to compare to this instance. |

### Return Value

a flag indicating whether this instance is equal to the specified object.

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


