---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt de horizontale resolutie op in dpi of stelt deze in"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Haalt op of stelt de horizontale resolutie in dpi in.

```csharp
public float HorizontalResolution { get; set; }
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


