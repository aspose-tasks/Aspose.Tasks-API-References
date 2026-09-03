---
title: "Aspose::Tasks::Saving::PdfDigitalSignatureDetails::PdfDigitalSignatureDetails 생성자"
linktitle: "PdfDigitalSignatureDetails"
articleTitle: "PdfDigitalSignatureDetails"
second_title: "C++용 Aspose.Tasks"
description: "PdfDigitalSignatureDetails 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---

## PdfDigitalSignatureDetails {#pdfdigitalsignaturedetails}

PdfDigitalSignatureDetails 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::Saving::

```cpp
PdfDigitalSignatureDetails(const System::SharedPtr< System::Security::Cryptography::X509Certificates::X509Certificate2 > & certificate, const System::String & reason, const System::String & location, System::DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| 매개변수 | 설명 |
| --- | --- |
| certificate | 서명에 사용할 X509Certificate2 인스턴스입니다. |
| reason | 서명의 이유입니다. |
| location | 서명 위치입니다. |
| signatureDate | 서명 날짜입니다. |
| hashAlgorithm | 서명에 사용되는 해시 알고리즘입니다. |

