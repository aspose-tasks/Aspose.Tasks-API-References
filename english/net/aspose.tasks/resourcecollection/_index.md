---
title: Class ResourceCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ResourceCollection class. Represents a collection of Resource objects
type: docs
weight: 1750
url: /net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Represents a collection of [`Resource`](../resource/) objects.

```csharp
public class ResourceCollection : IList<Resource>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Gets the number of elements contained in the ResourceCollection. Read-only Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Gets the parent project of the ResourceCollection object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Adds new resource at the last position of a project resources collection. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Adds new resource at the last position of a project resources collection. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Adds new resource at the specified position of a project resources collection. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Direct clearing is not supported, this method just throw NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Returns a resource with the specified id. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Returns a resource with the specified Uid. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | This is the stub implementation of ICollection's Remove method, that only throws NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Converts the ResourceCollection object to a list of [`Resource`](../resource/) objects. |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


