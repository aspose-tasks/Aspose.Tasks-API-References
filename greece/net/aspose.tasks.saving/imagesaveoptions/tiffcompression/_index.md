---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα εφαρμοστεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF"
type: docs
weight: 90
url: /el/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα εφαρμοστεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Παρατηρήσεις

Έχει ισχύ μόνο κατά την αποθήκευση σε TIFF. Η προεπιλεγμένη τιμή είναι `LZW`.

## Παραδείγματα

Δείχνει πώς να ορίσετε τη συμπίεση TIFF των αρχείων εξόδου TIFF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Για να χειριστούμε τη συμπίεση TIFF, μπορούμε να χρησιμοποιήσουμε την ιδιότητα ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Δείτε επίσης

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


