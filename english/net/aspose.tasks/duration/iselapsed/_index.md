---
title: Duration.IsElapsed
second_title: Aspose.Tasks for .NET API Reference
description: Duration property. Gets a value indicating whether time unit is elapsed. The flag which determines whether this Duration instance is elapsed
type: docs
weight: 20
url: /net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

Gets a value indicating whether time unit is elapsed. The flag which determines whether this Duration instance is elapsed.

```csharp
public bool IsElapsed { get; }
```

## Examples

Shows how to parse a string from a specially formatted string.

```csharp
var project = new Project();

// examples of durations:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// where 1 - number of items (day, week, etc), d - day (h - hour, w - week) ? - estimated flag, e - elapsed flag

// try to parse an estimated duration
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// try to parse an estimated duration
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


