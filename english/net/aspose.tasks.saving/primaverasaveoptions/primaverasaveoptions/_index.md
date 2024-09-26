---
title: PrimaveraSaveOptions.PrimaveraSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraSaveOptions constructor. Initializes a new instance of the PrimaveraSaveOptions class
type: docs
weight: 10
url: /net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Initializes a new instance of the [`PrimaveraSaveOptions`](../) class.

```csharp
public PrimaveraSaveOptions()
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


