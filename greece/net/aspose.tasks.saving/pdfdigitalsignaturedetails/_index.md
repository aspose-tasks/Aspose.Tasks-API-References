---
title: "Κλάση PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Saving.PdfDigitalSignatureDetails. Περιέχει λεπτομέρειες για μια ψηφιακή υπογραφή PDF"
type: docs
weight: 2080
url: /el/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Περιέχει λεπτομέρειες για ψηφιακή υπογραφή PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PdfDigitalSignatureDetails`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Λαμβάνει ή ορίζει το πιστοποιητικό με το οποίο θα υπογραφεί. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Λαμβάνει ή ορίζει τον αλγόριθμο κατακερματισμού. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Λαμβάνει ή ορίζει την τοποθεσία υπογραφής. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Λαμβάνει ή ορίζει τον λόγο υπογραφής. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία υπογραφής. |

## Παρατηρήσεις

Προς το παρόν η ψηφιακή υπογραφή εγγράφων PDF είναι διαθέσιμη μόνο σε .NET 2.0 ή νεότερο.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις λεπτομέρειες ψηφιακής υπογραφής PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// δημιουργία λεπτομερειών υπογραφής PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // καθορίστε το πιστοποιητικό
    certificate, 
    // καθορίστε έναν λόγο υπογραφής
    "reason",
    // καθορίστε μια τοποθεσία υπογραφής
    "location", 
    // καθορίστε μια ημερομηνία υπογραφής
    new DateTime(2019, 1, 1), 
    // καθορίστε έναν αλγόριθμο κατακερματισμού της υπογραφής
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// ορίστε τις λεπτομέρειες ψηφιακής υπογραφής
options.DigitalSignatureDetails = signatureDetails;

// αποθηκεύστε το έργο με τις καθορισμένες λεπτομέρειες κρυπτογράφησης
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


