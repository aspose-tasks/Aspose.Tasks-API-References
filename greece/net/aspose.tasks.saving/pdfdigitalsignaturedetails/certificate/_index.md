---
title: "PdfDigitalSignatureDetails.Certificate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfDigitalSignatureDetails. Λαμβάνει ή ορίζει το πιστοποιητικό με το οποίο θα γίνει η υπογραφή."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/
---
## PdfDigitalSignatureDetails.Certificate property

Λαμβάνει ή ορίζει το πιστοποιητικό με το οποίο θα υπογραφεί.

```csharp
public X509Certificate2 Certificate { get; set; }
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


