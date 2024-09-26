---
title: Prj.DurationFormat
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The format for expressing the bulk duration
type: docs
weight: 300
url: /net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

The format for expressing the bulk duration.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Examples

Shows how to read/write Prj.DurationFormat property.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


