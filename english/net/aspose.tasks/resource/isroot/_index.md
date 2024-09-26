---
title: Resource.IsRoot
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets the flag indicating whether resource is a root resource. Root resource is a special resource which is intended to support internals of MS Projects formats and is not intended to be used directly from the users code
type: docs
weight: 470
url: /net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Gets the flag indicating whether resource is a root resource. Root resource is a special resource which is intended to support internals of MS Project's formats and is not intended to be used directly from the user's code.

```csharp
public virtual bool IsRoot { get; }
```

## Examples

Shows how to use IsRoot property to skip root resource.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### See Also

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


