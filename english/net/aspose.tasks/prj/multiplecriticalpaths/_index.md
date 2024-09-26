---
title: Prj.MultipleCriticalPaths
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether multiple critical paths are calculated
type: docs
weight: 530
url: /net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

Determines whether multiple critical paths are calculated.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## Examples

Shows how to read/write Prj.MultipleCriticalPaths property.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


