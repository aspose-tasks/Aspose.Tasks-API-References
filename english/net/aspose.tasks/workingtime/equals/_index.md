---
title: WorkingTime.Equals
second_title: Aspose.Tasks for .NET API Reference
description: WorkingTime method. Checks that the objects are equal
type: docs
weight: 40
url: /net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Checks that the objects are equal.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | Second object to compare. |

### Return Value

True if the objects are equal, false otherwise.

## Examples

Shows how to check working time equality.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// the equality of calendars is checked against to working time's from and to dates.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### See Also

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


