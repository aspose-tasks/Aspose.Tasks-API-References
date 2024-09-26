---
title: ResourceCollection.Clear
second_title: Aspose.Tasks for .NET API Reference
description: ResourceCollection method. Direct clearing is not supported this method just throw NotSupportedException
type: docs
weight: 50
url: /net/aspose.tasks/resourcecollection/clear/
---
## ResourceCollection.Clear method

Direct clearing is not supported, this method just throw NotSupportedException.

```csharp
public void Clear()
```

## Examples

Shows how to work with resource collections.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// add empty resource
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// add resource with a name
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// add resource before the resource with specified ID
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// get resource by id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// resource collections does not support Clear operation
// project.Resources.Clear();
// use next code sample instead
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### See Also

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


