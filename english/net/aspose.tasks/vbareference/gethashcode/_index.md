---
title: VbaReference.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: VbaReference method. Returns a hash code value for this VbaReference
type: docs
weight: 50
url: /net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Returns a hash code value for this [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Return Value

Returns a hash code value for this object.

## Examples

Shows how to get a hash code of a VBA reference.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// the hash code of a reference is a hash code of internal reference's GUID
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### See Also

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


