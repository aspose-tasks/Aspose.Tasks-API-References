---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PdfDigitalSignatureDetails. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PdfDigitalSignatureDetails."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πιστοποιητικό | X509Certificate2 | Το αντικείμενο X509Certificate2 για υπογραφή. |
| λόγος | String | Ο λόγος της υπογραφής. |
| τοποθεσία | String | Η τοποθεσία της υπογραφής. |
| signatureDate | DateTime | Η ημερομηνία της υπογραφής. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | Ο αλγόριθμος κατακερματισμού της υπογραφής. |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


