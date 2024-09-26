---
title: Duration.Parse
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Converts the specified string to the instance of Duration struct
type: docs
weight: 10
url: /net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Converts the specified string to the instance of [`Duration`](../) struct.

```csharp
public static Duration Parse(Project p, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| p | Project | the specified instance of [`Project`](../../project/) class to convert duration for. |
| value | String | the specified string to convert. |

### Return Value

Returns the converted instance of [`Duration`](../) struct.

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


