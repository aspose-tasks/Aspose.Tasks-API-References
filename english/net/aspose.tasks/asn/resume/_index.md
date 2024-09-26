---
title: Asn.Resume
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The date when assignment is resumed
type: docs
weight: 490
url: /net/aspose.tasks/asn/resume/
---
## Asn.Resume field

The date when assignment is resumed.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Examples

Shows how to read assignment's stop/resume dates.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Print resource assignment's stop and resume dates
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


