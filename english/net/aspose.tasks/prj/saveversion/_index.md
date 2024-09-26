---
title: Prj.SaveVersion
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The version of Microsoft Office Project from which a project file was saved
type: docs
weight: 620
url: /net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

The version of Microsoft Office Project from which a project file was saved.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Examples

Shows how to check project's save version and save date.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Display project version
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


