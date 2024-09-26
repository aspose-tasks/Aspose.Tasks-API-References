---
title: Gridline.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Gridline method. Returns a flag indicating whether this instance is equal to the specified object
type: docs
weight: 50
url: /net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Returns a flag indicating whether this instance is equal to the specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | the specified object to compare to this instance. |

### Return Value

a flag indicating whether this instance is equal to the specified object.

## Examples

Shows how to check an equality of gridlines.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// the equality of gridlines is checked against to gridline type.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// change the type
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### See Also

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


