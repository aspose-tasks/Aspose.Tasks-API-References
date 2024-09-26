---
title: Rsc.OvertimeRateFormat
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The units used by Microsoft Project to display the overtime rate
type: docs
weight: 520
url: /net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

The units used by Microsoft Project to display the overtime rate.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
```

## Examples

Shows how to read resource overtime values.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Display overtime related parameters for all resources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


