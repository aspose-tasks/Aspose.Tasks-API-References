---
title: Prj.TimescaleFinish
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The date that the timescale in the view finishes
type: docs
weight: 730
url: /net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

The date that the timescale in the view finishes.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Examples

Shows how to read/write Prj.TimescaleFinish property.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


