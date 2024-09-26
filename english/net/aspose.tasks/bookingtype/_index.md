---
title: Enum BookingType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BookingType enum. Specifies the booking type of a resource
type: docs
weight: 150
url: /net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Specifies the booking type of a resource.

```csharp
public enum BookingType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates the value was not defined in original project file. |
| Committed | `0` | Indicates Committed booking type. |
| Proposed | `1` | Indicates Proposed booking type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to read/write Asn.BookingType property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


