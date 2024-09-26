---
title: SaveOptions.NonWorkingTimeColor
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the nonworking time color
type: docs
weight: 110
url: /net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Gets or sets the non-working time color.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Examples

Shows how to set custom color for non working time.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


