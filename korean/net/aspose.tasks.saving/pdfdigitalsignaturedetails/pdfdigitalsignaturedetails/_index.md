---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfDigitalSignatureDetails 생성자. PdfDigitalSignatureDetails 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

[`PdfDigitalSignatureDetails`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 인증서 | X509Certificate2 | 서명에 사용할 X509Certificate2 인스턴스입니다. |
| 이유 | 문자열 | 서명의 이유. |
| 위치 | 문자열 | 서명의 위치. |
| signatureDate | DateTime | 서명 날짜. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | 서명에 사용되는 해시 알고리즘. |

## 예제

PDF 디지털 서명 세부 정보를 다루는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// PDF 서명 세부 정보 만들기
var signatureDetails = new PdfDigitalSignatureDetails(
    // 인증서 지정
    certificate, 
    // 서명 이유 지정
    "reason",
    // 서명 위치 지정
    "location", 
    // 서명 날짜 지정
    new DateTime(2019, 1, 1), 
    // 서명 해시 알고리즘 지정
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// 디지털 서명 세부 정보 설정
options.DigitalSignatureDetails = signatureDetails;

// 지정된 암호화 세부 정보를 사용하여 프로젝트를 저장합니다
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### 또 보기

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


