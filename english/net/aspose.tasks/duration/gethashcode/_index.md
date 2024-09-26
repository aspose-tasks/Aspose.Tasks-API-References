---
title: Duration.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Returns a hash code value for this object
type: docs
weight: 90
url: /net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Returns a hash code value for this object.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this duration instance.

## Examples

Shows how to get a hash code of a duration.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// the hash code of a calendar is based on time unit type and initial value of duration
// so next hash codes are equal
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// but hash codes of duration 1 and 3 is not
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


