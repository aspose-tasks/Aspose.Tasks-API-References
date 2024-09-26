---
title: ReadOnlyCollectionBase1.Count
second_title: Aspose.Tasks for .NET API Reference
description: ReadOnlyCollectionBase property. Gets the number of objects contained in the object
type: docs
weight: 10
url: /net/aspose.tasks/readonlycollectionbase-1/count/
---
## ReadOnlyCollectionBase&lt;T&gt;.Count property

Gets the number of objects contained in the object.

```csharp
public int Count { get; }
```

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


