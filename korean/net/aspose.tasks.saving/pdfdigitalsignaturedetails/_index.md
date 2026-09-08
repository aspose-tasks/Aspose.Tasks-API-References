---
title: "클래스 PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureDetails 클래스. PDF 디지털 서명에 대한 세부 정보를 포함합니다."
type: docs
weight: 2080
url: /ko/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

PDF 디지털 서명에 대한 세부 정보를 포함합니다.

```csharp
public class PdfDigitalSignatureDetails
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | `PdfDigitalSignatureDetails` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | 서명에 사용할 인증서를 가져오거나 설정합니다. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | 해시 알고리즘을 가져오거나 설정합니다. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | 서명 위치를 가져오거나 설정합니다. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | 서명 이유를 가져오거나 설정합니다. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | 서명 날짜를 가져오거나 설정합니다. |

## 비고

현재 PDF 문서에 디지털 서명하는 기능은 .NET 2.0 이상에서만 사용할 수 있습니다.

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


