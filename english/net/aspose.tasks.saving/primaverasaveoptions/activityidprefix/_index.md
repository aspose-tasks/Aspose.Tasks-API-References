---
title: PrimaveraSaveOptions.ActivityIdPrefix
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraSaveOptions property. Gets or sets the prefix used in renumbering of activity IDs
type: docs
weight: 30
url: /net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

Gets or sets the prefix used in renumbering of activity IDs.

```csharp
public string ActivityIdPrefix { get; set; }
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


