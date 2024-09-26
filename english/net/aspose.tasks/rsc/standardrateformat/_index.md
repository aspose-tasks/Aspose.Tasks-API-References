---
title: Rsc.StandardRateFormat
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The units used by Microsoft Project to display the standard rate
type: docs
weight: 630
url: /net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

The units used by Microsoft Project to display the standard rate.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Examples

Shows how to read/write Rsc.StandardRateFormat property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


