---
title: PrimaveraSaveOptions.ActivityIdSuffix
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraSaveOptions property. Gets or sets the suffix used in renumbering of activity IDs
type: docs
weight: 40
url: /net/aspose.tasks.saving/primaverasaveoptions/activityidsuffix/
---
## PrimaveraSaveOptions.ActivityIdSuffix property

Gets or sets the suffix used in renumbering of activity IDs.

```csharp
public int ActivityIdSuffix { get; set; }
```

## Examples

Shows how to work with &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// create Primavera save options and tune them
var options = new PrimaveraSaveOptions
                  {
                      // define prefix and suffix of an activity
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // control renumbering of activities
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### See Also

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


