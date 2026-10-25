---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions-eigenschap. Haalt op of stelt de verticale resolutie in dpi in."
type: docs
weight: 100
url: /nl/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Haalt op of stelt de verticale resolutie in dpi in.

```csharp
public float VerticalResolution { get; set; }
```

## Voorbeelden

Toont hoe het pixelformaat in te stellen dat wordt gebruikt tijdens de conversie naar afbeeldingsformaten.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Zie ook

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


