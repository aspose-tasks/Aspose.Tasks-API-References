---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions constructor. Initialiseert een nieuw exemplaar van de ImageSaveOptions‑klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-formaten."
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`ImageSaveOptions`](../) klasse die kan worden gebruikt om gerenderde afbeeldingen op te slaan in TIFF-, PNG-, BMP- of JPEG-formaten.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Kan TIFF, PNG, BMP of JPEG[`SaveFileFormat`](../../savefileformat/) zijn. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Goedgegooid wanneer *saveFormat* geen geldig afbeeldingsformaat is. De geldige waarden zijn TIFF, PNG, BMP of JPEG. |

## Voorbeelden

Toont hoe een project kan worden opgeslagen in een stream als afbeelding.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // door gebruik te maken van ImageSaveOptions slaan we het project op in een afbeeldingsformaat
    project.Save(stream, options);
}
```

### Zie ook

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


