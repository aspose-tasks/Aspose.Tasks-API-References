---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PdfEncryptionDetails. Αρχικοποιεί μια νέα παρουσία της κλάσης PdfEncryptionDetails."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| userPassword | String | Ο κωδικός πρόσβασης χρήστη που επιτρέπει το άνοιγμα προστατευμένων εγγράφων. |
| ownerPassword | String | Ο κωδικός πρόσβασης ιδιοκτήτη που επιτρέπει το άνοιγμα προστατευμένων εγγράφων. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | Η παρουσία του [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) που υποδεικνύει τον αλγόριθμο κρυπτογράφησης. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


