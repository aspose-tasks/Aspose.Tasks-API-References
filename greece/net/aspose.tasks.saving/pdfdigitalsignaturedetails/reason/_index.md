---
title: "PdfDigitalSignatureDetails.Reason"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfDigitalSignatureDetails. Λαμβάνει ή ορίζει το λόγο υπογραφής."
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/pdfdigitalsignaturedetails/reason/
---
## PdfDigitalSignatureDetails.Reason property

Λαμβάνει ή ορίζει τον λόγο υπογραφής.

```csharp
public string Reason { get; set; }
```

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

* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


