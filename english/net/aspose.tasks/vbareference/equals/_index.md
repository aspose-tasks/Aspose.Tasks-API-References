---
title: VbaReference.Equals
second_title: Aspose.Tasks for .NET API Reference
description: VbaReference method. Returns a value indicating whether this instance is equal to the specified VbaReference object
type: docs
weight: 40
url: /net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Returns a value indicating whether this instance is equal to the specified [`VbaReference`](../) object.

```csharp
public bool Equals(VbaReference other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | VbaReference | The specified [`VbaReference`](../) object to compare with this instance. |

### Return Value

Returns true if this instance is equal to the specified [`VbaReference`](../) object; otherwise, false.

## Examples

Shows how to check VBA reference equality.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// the equality of references is checked against to reference's name.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### See Also

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to the specified [`VbaReference`](../) object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified [`VbaReference`](../) object to compare with this instance. |

### Return Value

Returns true if this instance is equal to the specified [`VbaReference`](../) object; otherwise, false.

## Examples

Shows how to check VBA reference equality.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// the equality of references is checked against to reference's name.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### See Also

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


