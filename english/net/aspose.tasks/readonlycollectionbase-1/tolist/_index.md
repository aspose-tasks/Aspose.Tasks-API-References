---
title: ReadOnlyCollectionBase1.ToList
second_title: Aspose.Tasks for .NET API Reference
description: ReadOnlyCollectionBase method. Converts the collection object to a list of VbaModule objects
type: docs
weight: 50
url: /net/aspose.tasks/readonlycollectionbase-1/tolist/
---
## ReadOnlyCollectionBase&lt;T&gt;.ToList method

Converts the collection object to a list of [`VbaModule`](../../vbamodule/) objects.

```csharp
public List<T> ToList()
```

### Return Value

List of objects.

## Examples

Shows how to iterate over VBA modules.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (var module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}

// the collection can be converted into a plain list
List<VbaModule> modules = vbaProject.Modules.ToList();
foreach (var unused in modules)
{
    // work with modules
}
```

### See Also

* class [ReadOnlyCollectionBase&lt;T&gt;](../)
* namespace [Aspose.Tasks](../../readonlycollectionbase-1/)
* assembly [Aspose.Tasks](../../../)


