---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfEncryptionDetails. Λαμβάνει ή ορίζει τον κωδικό πρόσβασης Owner."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

Λαμβάνει ή ορίζει τον κωδικό πρόσβασης Owner.

```csharp
public string OwnerPassword { get; set; }
```

## Παρατηρήσεις

Το άνοιγμα του εγγράφου με τον σωστό κωδικό πρόσβασης ιδιοκτήτη (υποθέτοντας ότι δεν είναι ίδιος με τον κωδικό πρόσβασης χρήστη) επιτρέπει πλήρη (ιδιοκτήτη) πρόσβαση στο έγγραφο. Αυτή η απεριόριστη πρόσβαση περιλαμβάνει τη δυνατότητα αλλαγής των κωδικών πρόσβασης του εγγράφου και των δικαιωμάτων πρόσβασης.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


