---
title: "Aspose::Tasks::Saving::PdfDigitalSignatureDetails::PdfDigitalSignatureDetails constructor"
linktitle: "PdfDigitalSignatureDetails"
articleTitle: "PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for C++"
description: "Initializes a new instance of the PdfDigitalSignatureDetails class."
type: docs
weight: 10
url: /cpp/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---

## PdfDigitalSignatureDetails {#pdfdigitalsignaturedetails}

Initializes a new instance of the PdfDigitalSignatureDetails class.

**Returns:** Aspose::Tasks::Saving::

```cpp
PdfDigitalSignatureDetails(const System::SharedPtr< System::Security::Cryptography::X509Certificates::X509Certificate2 > & certificate, const System::String & reason, const System::String & location, System::DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parameter | Description |
| --- | --- |
| certificate | The X509Certificate2 instance to sign with. |
| reason | The reason of signing. |
| location | The location of signing. |
| signatureDate | The date of signing. |
| hashAlgorithm | The hash algorithm of signing. |

