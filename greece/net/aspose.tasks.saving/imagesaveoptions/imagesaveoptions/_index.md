---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ImageSaveOptions. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης ImageSaveOptions που μπορεί να χρησιμοποιηθεί για την αποθήκευση αποδιδόμενων εικόνων σε μορφές TIFF, PNG, BMP ή JPEG."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ImageSaveOptions`](../) που μπορεί να χρησιμοποιηθεί για την αποθήκευση αποδιδόμενων εικόνων σε μορφές TIFF, PNG, BMP ή JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Μπορεί να είναι TIFF, PNG, BMP ή JPEG[`SaveFileFormat`](../../savefileformat/). |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Εκτοπίζεται εάν το *saveFormat* δεν είναι έγκυρη μορφή εικόνας. Οι έγκυρες τιμές είναι TIFF, PNG, BMP ή JPEG. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο σε ροή ως εικόνα.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // χρησιμοποιώντας το ImageSaveOptions αποθηκεύουμε το έργο σε μορφή εικόνας
    project.Save(stream, options);
}
```

### Δείτε επίσης

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


