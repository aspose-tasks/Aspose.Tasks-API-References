---
title: Resource.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Resource method. Returns a value indicating whether this instance is equal to a specified instance of the Resource class
type: docs
weight: 820
url: /net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Returns a value indicating whether this instance is equal to a specified instance of the [`Resource`](../) class.

```csharp
public bool Equals(Resource other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | Resource | The specified instance of the [`Resource`](../) class to compare with this instance. |

### Return Value

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Examples

Shows how to check resource equality.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### See Also

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Examples

Shows how to check resource equality.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### See Also

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


