---
title: Prj.TimescaleStart
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The date that the timescale in the view starts
type: docs
weight: 740
url: /net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

The date that the timescale in the view starts.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Examples

Shows how to set timescale start date to tune the date where the view should start.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


