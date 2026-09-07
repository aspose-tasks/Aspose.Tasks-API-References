---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore ImageSaveOptions. Inizializza una nuova istanza della classe ImageSaveOptions che può essere usata per salvare immagini renderizzate nei formati TIFF, PNG, BMP o JPEG"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Inizializza una nuova istanza della classe [`ImageSaveOptions`](../) che può essere usata per salvare immagini renderizzate nei formati TIFF, PNG, BMP o JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Può essere TIFF, PNG, BMP o JPEG[`SaveFileFormat`](../../savefileformat/). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Generato se *saveFormat* non è un formato immagine valido. I valori validi sono TIFF, PNG, BMP o JPEG. |

## Esempi

Mostra come salvare il progetto in uno stream come immagine.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // utilizzando ImageSaveOptions salviamo il progetto in formato immagine
    project.Save(stream, options);
}
```

### Vedi anche

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


