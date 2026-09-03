---
title: "Aspose::Tasks::Saving::PdfDigitalSignatureDetails::PdfDigitalSignatureDetails constructor"
linktitle: "PdfDigitalSignatureDetails"
articleTitle: "PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for C++"
description: "Inicializa una nueva instancia de la clase PdfDigitalSignatureDetails."
type: docs
weight: 10
url: /es/cpp/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---

## PdfDigitalSignatureDetails {#pdfdigitalsignaturedetails}

Inicializa una nueva instancia de la clase PdfDigitalSignatureDetails.

**Returns:** Aspose::Tasks::Saving::

```cpp
PdfDigitalSignatureDetails(const System::SharedPtr< System::Security::Cryptography::X509Certificates::X509Certificate2 > & certificate, const System::String & reason, const System::String & location, System::DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Parámetro | Descripción |
| --- | --- |
| certificado | La instancia X509Certificate2 con la que firmar. |
| razón | La razón de la firma. |
| ubicación | La ubicación de la firma. |
| signatureDate | La fecha de la firma. |
| hashAlgorithm | El algoritmo de hash de la firma. |

