---
title: VbaModuleAttribute.Equals
second_title: Aspose.Tasks for .NET API Reference
description: VbaModuleAttribute method. Returns a value indicating whether this instance is equal to the specified VbaModuleAttribute object
type: docs
weight: 30
url: /net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Returns a value indicating whether this instance is equal to the specified [`VbaModuleAttribute`](../) object.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | VbaModuleAttribute | The specified [`VbaModuleAttribute`](../) object to compare with this instance. |

### Return Value

Returns true if this instance is equal to the specified [`VbaModuleAttribute`](../) object; otherwise, false.

## Examples

Shows how to check VBA module attributes equality.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### See Also

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to the specified [`VbaModuleAttribute`](../) object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified [`VbaModuleAttribute`](../) object to compare with this instance. |

### Return Value

Returns true if this instance is equal to the specified [`VbaModuleAttribute`](../) object; otherwise, false.

## Examples

Shows how to check VBA module attributes equality.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### See Also

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


