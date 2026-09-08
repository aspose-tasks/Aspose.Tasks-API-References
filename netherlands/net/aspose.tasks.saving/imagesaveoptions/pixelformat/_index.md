---
title: "ImageSaveOptions.PixelFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt het formaat van de kleurgegevens voor elke pixel in de afbeelding op of stelt dit in."
type: docs
weight: 70
url: /nl/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Haalt op of stelt het formaat van de kleurgegevens voor elke pixel in de afbeelding in.

```csharp
public PixelFormat PixelFormat { get; set; }
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


