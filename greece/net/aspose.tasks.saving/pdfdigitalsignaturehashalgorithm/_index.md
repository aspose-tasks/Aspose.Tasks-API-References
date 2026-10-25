---
title: "Απαρίθμηση PdfDigitalSignatureHashAlgorithm"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm απαρίθμηση. Καθορίζει τον αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από την ψηφιακή υπογραφή"
type: docs
weight: 2090
url: /el/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Καθορίζει τον αλγόριθμο ψηφιακού κατακερματισμού που χρησιμοποιείται από την ψηφιακή υπογραφή.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Sha1 | `0` | Καθορίζει έναν αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από μια ψηφιακή υπογραφή. |
| Sha256 | `1` | Καθορίζει έναν αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από μια ψηφιακή υπογραφή. |
| Sha384 | `2` | Καθορίζει έναν αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από μια ψηφιακή υπογραφή. |
| Sha512 | `3` | Καθορίζει έναν αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από μια ψηφιακή υπογραφή. |
| Md5 | `4` | Καθορίζει έναν αλγόριθμο ψηφιακής κατακερματισμού που χρησιμοποιείται από μια ψηφιακή υπογραφή. |

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


