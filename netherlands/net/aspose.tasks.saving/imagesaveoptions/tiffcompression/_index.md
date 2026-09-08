---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt het type compressie op of stelt dit in dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat"
type: docs
weight: 90
url: /nl/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Haalt op of stelt het type compressie in dat moet worden toegepast bij het opslaan van gegenereerde afbeeldingen in het TIFF‑formaat.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Opmerkingen

Heeft alleen effect bij het opslaan naar TIFF. De standaardwaarde is `LZW`.

## Voorbeelden

Toont hoe je de TIFF-compressie van de uitvoer‑TIFF‑bestanden instelt.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Om TIFF-compressie te manipuleren kunnen we de ImageSaveOptions.TiffCompression eigenschap gebruiken.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Zie ook

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


