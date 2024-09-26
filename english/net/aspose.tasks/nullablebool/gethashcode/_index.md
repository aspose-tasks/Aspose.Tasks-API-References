---
title: NullableBool.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool method. Returns a hash code value for the instance of the NullableBool class
type: docs
weight: 50
url: /net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Returns a hash code value for the instance of the [`NullableBool`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to work with &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode method.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// the hash code of bools is based on 'IsDefined' and 'Value' properties
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### See Also

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


