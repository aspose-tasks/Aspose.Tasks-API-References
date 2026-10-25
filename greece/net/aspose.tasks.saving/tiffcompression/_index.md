---
title: "Enum TiffCompression"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.TiffCompression enum. Καθορίζει ποιος τύπος συμπίεσης θα εφαρμοστεί όταν αποθηκεύονται σελίδες σε μορφή TIFF"
type: docs
weight: 2250
url: /el/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Καθορίζει ποιος τύπος συμπίεσης θα εφαρμοστεί κατά την αποθήκευση σελίδων σε μορφή TIFF.

```csharp
public enum TiffCompression
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `1` | Καθορίζει καμία συμπίεση. |
| Rle | `2` | Καθορίζει το σχήμα συμπίεσης RLE. |
| Ccitt3 | `3` | Καθορίζει το σχήμα συμπίεσης CCITT3. |
| Ccitt4 | `4` | Καθορίζει το σχήμα συμπίεσης CCITT4. |
| Lzw | `5` | Καθορίζει το σχήμα συμπίεσης LZW. |

## Παραδείγματα

Δείχνει πώς να αποδώσετε σε μορφή TIFF χρησιμοποιώντας τη λειτουργία συμπίεσης RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Αποθηκεύστε το έργο με συμπίεση Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


