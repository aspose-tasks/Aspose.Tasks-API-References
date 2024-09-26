---
title: Project.Get
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Returns the value to which the property is mapped in this container
type: docs
weight: 1070
url: /net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Returns the value to which the property is mapped in this container.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parameter | Description |
| --- | --- |
| T | the type of the mapped value. |
| key | the specified property key. [`Prj`](../../prj/) for getting the property key. |

### Return Value

the value to which the property is mapped in this container.

## Examples

Shows how to check a project version.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Display project version
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


