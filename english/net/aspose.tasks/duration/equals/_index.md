---
title: Duration.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 80
url: /net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public bool Equals(Duration other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | Duration | The object to compare with this instance. |

### Return Value

Returns **True** if other Duration instance has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


