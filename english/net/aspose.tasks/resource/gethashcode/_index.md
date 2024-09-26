---
title: Resource.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: Resource method. Returns a hash code value for the instance of the Resource class
type: docs
weight: 840
url: /net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Returns a hash code value for the instance of the [`Resource`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to get a hash code of a resource.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// the hash code of a resource is equal to resource UID 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### See Also

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


