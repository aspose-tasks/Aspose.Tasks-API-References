---
title: "Enum PdfPermissions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η απαρίθμηση Aspose.Tasks.Saving.PdfPermissions. Καθορίζει τα δικαιώματα που χρησιμοποιούνται για την πρόσβαση σε ένα έγγραφο PDF"
type: docs
weight: 2120
url: /el/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF.

```csharp
public enum PdfPermissions
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| Printing | `4` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| ModifyContents | `8` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| ContentCopy | `16` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| ModifyAnnotations | `32` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| FillIn | `256` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| ContentCopyForAccessibility | `512` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| DocumentAssembly | `1024` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| HighResolutionPrinting | `2052` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |
| AllowAll | `65535` | Καθορίζει τα δικαιώματα που θα χρησιμοποιηθούν για την πρόσβαση σε έγγραφο PDF. |

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


