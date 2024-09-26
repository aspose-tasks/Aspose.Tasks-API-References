---
title: Duration.op_Equality
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 140
url: /net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public static bool operator ==(Duration a, Duration b)
```

| Parameter | Type | Description |
| --- | --- | --- |
| a | Duration | The first duration. |
| b | Duration | The second duration. |

### Return Value

a value indicating whether this instance is equal to a specified object

## Examples

Shows how to check duration equality.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// the equality of duration is checked against to underlying timespan
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


