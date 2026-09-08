---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다."
type: docs
weight: 2090
url: /ko/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Sha1 | `0` | 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다. |
| Sha256 | `1` | 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다. |
| Sha384 | `2` | 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다. |
| Sha512 | `3` | 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다. |
| Md5 | `4` | 디지털 서명에 사용되는 디지털 해시 알고리즘을 지정합니다. |

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


