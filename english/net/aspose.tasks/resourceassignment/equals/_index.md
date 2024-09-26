---
title: ResourceAssignment.Equals
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Returns a value indicating whether this instance is equal to a specified instance of the ResourceAssignment class
type: docs
weight: 690
url: /net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Returns a value indicating whether this instance is equal to a specified instance of the [`ResourceAssignment`](../) class.

```csharp
public bool Equals(ResourceAssignment other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | ResourceAssignment | The specified instance of the [`ResourceAssignment`](../) class to compare with this instance. |

### Return Value

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Examples

Shows how to check resource assignment equality.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Examples

Shows how to check resource assignment equality.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


