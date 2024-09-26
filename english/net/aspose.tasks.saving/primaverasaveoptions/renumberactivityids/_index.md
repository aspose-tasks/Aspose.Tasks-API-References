---
title: PrimaveraSaveOptions.RenumberActivityIds
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraSaveOptions property. Gets or sets a value indicating whether is need to renumbers activity IDs
type: docs
weight: 50
url: /net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Gets or sets a value indicating whether is need to renumbers activity IDs.

```csharp
public bool RenumberActivityIds { get; set; }
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


