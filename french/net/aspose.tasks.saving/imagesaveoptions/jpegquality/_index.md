---
title: "ImageSaveOptions.JpegQuality"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit la qualité JPEG. La plage de valeurs autorisée est 0..100"
type: docs
weight: 40
url: /fr/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Obtient ou définit la qualité JPEG. La plage de valeurs autorisée est 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Exemples

Montre comment définir la qualité JPEG des fichiers JPEG de sortie.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Pour manipuler la qualité JPEG, on peut utiliser la propriété ImageSaveOptions.JpegQuality.
// La plage de valeurs autorisée est 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Voir aussi

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


