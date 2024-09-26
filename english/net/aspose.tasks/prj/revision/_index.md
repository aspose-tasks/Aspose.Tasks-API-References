---
title: Prj.Revision
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The number of times a project was saved
type: docs
weight: 610
url: /net/aspose.tasks/prj/revision/
---
## Prj.Revision field

The number of times a project was saved.

```csharp
public static readonly Key<int, PrjKey> Revision;
```

## Examples

Shows how to set project meta information.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Set project information
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


