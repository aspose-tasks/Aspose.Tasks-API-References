---
title: Prj.LastSaved
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The date when a project was saved last time. Saved in UTC format in mpp files. DateTime type
type: docs
weight: 440
url: /net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

The date when a project was saved last time. Saved in UTC format in mpp files. DateTime type.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


