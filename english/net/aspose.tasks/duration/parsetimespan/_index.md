---
title: Duration.ParseTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Parses duration string in format PTHMS
type: docs
weight: 130
url: /net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Parses duration string in format "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | String | the specified string to parse. |

### Return Value

returns parsed instance of the [`TimeSpan`](../timespan/) struct.

## Examples

Shows how to convert a string into a time span.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


