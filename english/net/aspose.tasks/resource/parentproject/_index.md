---
title: Resource.ParentProject
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets parent project for this container
type: docs
weight: 600
url: /net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Gets parent project for this container.

```csharp
public Project ParentProject { get; }
```

## Examples

Shows how to use parent project of resource.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// set a work for the resource by using default project work time unit type.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### See Also

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


