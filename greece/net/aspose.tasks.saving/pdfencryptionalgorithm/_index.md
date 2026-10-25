---
title: "Απαρίθμηση PdfEncryptionAlgorithm"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.PdfEncryptionAlgorithm απαρίθμηση. Καθορίζει τον αλγόριθμο κρυπτογράφησης που θα χρησιμοποιηθεί για την κρυπτογράφηση ενός εγγράφου PDF"
type: docs
weight: 2100
url: /el/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

Καθορίζει τον αλγόριθμο κρυπτογράφησης που θα χρησιμοποιηθεί για την κρυπτογράφηση ενός εγγράφου PDF.

```csharp
public enum PdfEncryptionAlgorithm
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| RC4_40 | `0` | Καθορίζει τον αλγόριθμο κρυπτογράφησης που θα χρησιμοποιηθεί για την κρυπτογράφηση ενός εγγράφου PDF. |
| RC4_128 | `1` | Καθορίζει τον αλγόριθμο κρυπτογράφησης που θα χρησιμοποιηθεί για την κρυπτογράφηση ενός εγγράφου PDF. |

## Παραδείγματα

Δείχνει πώς να καθορίσετε λεπτομέρειες κρυπτογράφησης PDF κατά την αποθήκευση ενός έργου ως αρχείο PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Αφήνουμε να καθορίσουμε λεπτομέρειες κρυπτογράφησης
var encryptionDetails = new PdfEncryptionDetails(
    // καθορίστε κωδικό πρόσβασης User
    "userPassword", 
    // καθορίστε κωδικό πρόσβασης Owner
    "ownerPassword", 
    // καθορίστε αλγόριθμο κρυπτογράφησης
    PdfEncryptionAlgorithm.RC4_128);

// καθορίστε δικαιώματα
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// εμφανίστε κωδικούς πρόσβασης User και Owner
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// εμφανίστε λειτουργία κρυπτογράφησης: RC4_40 ή RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// αποθηκεύστε το έργο με τις καθορισμένες λεπτομέρειες κρυπτογράφησης
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


