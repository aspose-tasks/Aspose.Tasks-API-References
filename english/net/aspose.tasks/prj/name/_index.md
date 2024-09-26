---
title: Prj.Name
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The name of the project
type: docs
weight: 540
url: /net/aspose.tasks/prj/name/
---
## Prj.Name field

The name of the project.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Examples

Shows how to read/write project name.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


