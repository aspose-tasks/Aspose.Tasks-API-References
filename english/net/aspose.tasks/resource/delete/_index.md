---
title: Resource.Delete
second_title: Aspose.Tasks for .NET API Reference
description: Resource method. Deletes a resource and its assignments from project
type: docs
weight: 810
url: /net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Deletes a resource and its assignments from project.

```csharp
public void Delete()
```

## Examples

Shows how to delete a resource.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// delete the resource
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### See Also

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


